# Infosys Off-Campus Drive – Preparation Resources & Sample Questions

## Email Received

**From:** Talent Acquisition Team, Infosys Limited

---

Dear Candidate,

Warm greetings from Infosys!

At Infosys, we are committed to amplifying human potential and creating opportunities that transform individuals, businesses, and communities. As a global leader in next-generation AI-first digital services and consulting, we proudly serve 1,800+ clients across 50+ countries, powered by a workforce of over 300,000 professionals.

Thank you for applying to our upcoming Off-Campus Drive.

To help you prepare with confidence, we are sharing curated resources designed to sharpen your technical foundation and build job-ready skills.

---

# Selection Process

The recruitment process consists of **two stages**:

## Round 1 – Virtual Assessment

- Online assessment
- Conducted remotely

## Round 2 – In-Person Assessment & Interview

Candidates shortlisted from Round 1 will be invited for:

- Physical assessment
- Technical interview
- HR interview (if applicable)

---

# Preparation Resources

Infosys recommends attending the following sessions:

### 1. Orientation Session

**Upgrade Program**

- Infosys Power Programmer Hiring Explained
- Mock Questions Solved

---

### 2. Navigator Session 1

Topics:

- Assessment Strategy
- Core Data Structures & Algorithms

---

### 3. Navigator Session 2

Topics:

- Graphs
- Dynamic Programming
- Competitive Coding

---

Sample question papers are also attached to help candidates understand the assessment pattern.

---

# Important Note

This is a fresh start—and Infosys is here to support you throughout your preparation journey.

Stay consistent, utilise the preparation resources, and approach the assessment with confidence.

---

# Disclaimer

Infosys:

- Does **NOT** charge candidates at any stage of recruitment.
- Does **NOT** recruit through external vendors.
- Candidates should stay alert against fraudulent recruitment communications.

---

# Sample Questions

---

# Easy Problem

## Food Stamps

### Problem Statement

You want to buy food from a store.

Each food type has an initial taste value.

If you buy the same food multiple times, the taste decreases.

For the **ti-th** purchase of food **i**, the taste obtained is:

```
v[i] - d[i] × (ti - 1)
```

You may purchase at most **M meals** in total.

Find the maximum taste points obtainable.

---

## Input Format

```
N
M
v1
v2
...
vN
d1
d2
...
dN
```

---

## Constraints

```
1 ≤ N ≤ 100000
1 ≤ M ≤ 10^9
1 ≤ v[i] ≤ 10^9
1 ≤ d[i] ≤ 10^9
```

---

## Sample Test Case 1

### Input

```
1
1
5
2
```

### Output

```
5
```

Explanation:

Buy the only food once.

---

## Sample Test Case 2

### Input

```
2
2
5
7
2
4
```

### Output

```
12
```

Explanation:

Buy each food once.

```
5 + 7 = 12
```

---

## Sample Test Case 3

### Input

```
3
5
5
7
9
2
4
6
```

### Output

```
27
```

Explanation

Food 1:

```
5 + (5-2)=8
```

Food 2:

```
7 + (7-4)=10
```

Food 3:

```
9
```

Total

```
8 + 10 + 9 = 27
```

---

# Medium Problem

## MSS With Swaps

### Problem Statement

Given an array **A** and integer **K**.

Perform exactly **K swaps**.

A swap exchanges two array elements.

Find the maximum possible **Maximum Subarray Sum (MSS)** after the swaps.

Since swapping the same pair twice cancels the effect,

"Exactly K swaps"

is equivalent to

"At most K useful swaps."

---

## Input Format

```
N
K
A1
A2
...
AN
```

---

## Constraints

```
2 ≤ N ≤ 500
0 ≤ K ≤ N
-1000 ≤ A[i] ≤ 1000
```

---

## Sample Test Case 1

Input

```
3
1
1
-5
2
```

Output

```
3
```

Explanation

Swap

```
1
```

and

```
-5
```

New array

```
-5 1 2
```

Maximum subarray

```
1 + 2 = 3
```

---

## Sample Test Case 2

Input

```
3
0
5
-1
5
```

Output

```
9
```

Entire array is already the maximum subarray.

---

## Sample Test Case 3

Input

```
3
0
1
-5
2
```

Output

```
2
```

Maximum subarray is

```
[2]
```

---

# Hard Problem

## Lock & Parity

### Problem Statement

There are **N locks**.

Each lock has one key underneath it.

Rules:

1. Key **j** can only unlock lock **i** if

```
j < i
```

2. Values must be different.

```
L[j] ≠ L[i]
```

3. Cost

```
|L[j] - L[i]|
```

4. Every key and lock can be used at most once.

5. Let

```
even = number of assignments with even cost

odd = number of assignments with odd cost
```

Valid only if

```
even ≥ odd
```

6. At least one assignment is required.

Find the minimum total cost.

If impossible,

```
-1
```

---

## Constraints

```
1 ≤ N ≤ 200
1 ≤ L[i] ≤ 100000
```

---

## Sample Test Case 1

Input

```
6
41
54
15
4
54
4
```

Output

```
26
```

Explanation

Choose assignment

```
1 → 3
```

Cost

```
26
```

Even assignments = 1

Odd assignments = 0

Valid.

---

## Sample Test Case 2

Input

```
6
45
6
38
6
15
38
```

Output

```
30
```

Choose

```
1 → 5
```

Cost

```
30
```

---

## Sample Test Case 3

Input

```
6
6
59
1
25
59
50
```

Output

```
24
```

Choose

```
3 → 4
```

Cost

```
24
```

---

# Complex Problem

## Layer-Split Path Maximization with Penalties

### Problem Statement

Given an undirected graph.

Each node has:

- Layer
- Value

Choose a **simple path** satisfying:

Layer order must be non-decreasing.

```
L1 ≤ L2 ≤ L3 ...
```

Whenever the layer increases,

Penalty

```
(newLayer - oldLayer)^2
```

Final score

```
Sum(Node Values)
-
Sum(Penalties)
```

Find the maximum possible score.

---

## Input Format

```
N
M
K

N lines:
Layer Value

M lines:
u v
```

---

## Constraints

```
1 ≤ N ≤ 100000
1 ≤ M ≤ 100000
1 ≤ K ≤ 100000

-10^9 ≤ Value ≤ 10^9
```

---

## Sample Test Case 1

Input

```
2
1
10

1 10
3 100

0 1
```

Output

```
106
```

Explanation

Path

```
0 → 1
```

Value

```
110
```

Penalty

```
(3-1)^2 = 4
```

Score

```
110 - 4 = 106
```

---

## Sample Test Case 2

Input

```
3
2
3

1 10
2 20
3 30

0 1
1 2
```

Output

```
58
```

Explanation

Path

```
0 → 1 → 2
```

Value

```
60
```

Penalty

```
1 + 1 = 2
```

Final

```
58
```

---

## Sample Test Case 3

Input

```
3
2
3

1 -5
2 100
3 -10

0 1
1 2
```

Output

```
100
```

Explanation

Best path consists of only node

```
1
```

Value

```
100
```

No penalty.

---

# Topics Covered

The sample paper tests the following concepts:

## Easy

- Greedy
- Priority Queue
- Mathematical Optimisation

## Medium

- Kadane's Algorithm
- Swapping Optimisation
- Dynamic Programming

## Hard

- Graph Matching
- Dynamic Programming
- Minimum Cost Matching
- Parity Constraints

## Complex

- Graph Theory
- DAG DP
- Longest Path
- Dynamic Programming
- Layered Graph Optimisation

---

# Preparation Tips

- Revise Data Structures & Algorithms.
- Practise Dynamic Programming.
- Solve Graph problems regularly.
- Strengthen Greedy techniques.
- Revise Kadane's Algorithm.
- Practise competitive programming questions with time limits.
- Attempt mock assessments before the actual test.

---

**Best of luck with your Infosys Off-Campus Drive preparation!**


## Resource Link 2

https://prepinsta.com/infosys-sp-and-dse/coding-questions/?logout=1778634917050&fbclid=PARlRTSATTAcVwZG9mAmV4dG4DYWVtAjEwAHNydGMGYXBwX2lkDzEyNDAyNDU3NDI4NzQxNAABp_L_axlpWiLcmW614ZoDmX9vY0nA5OIdOWNqA3xy9adlCCwRlKoZ-1OCfaZk_aem_fQBanLqoYTEzjgZMnscfeQ


