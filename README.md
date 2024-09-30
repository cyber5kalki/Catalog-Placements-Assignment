# Catalog Placements Assignment

### Problem Description:
This project implements a simplified version of **Shamir's Secret Sharing** algorithm to compute the constant term `c` of a polynomial based on given roots in JSON format. The goal is to solve for `c` using the roots provided in the input and identify any incorrect points in the second test case.

### Technologies Used:
- **Language:** Used Programming Language **JavaScript**
- **Environment:** VS Code

### Problem Summary:
Given an unknown polynomial of degree `m`, we require `m + 1` roots (encoded in different bases) to solve for its coefficients. The task involves:
1. Reading input from a JSON file.
2. Decoding Y values (encoded in different bases).
3. Solving for the constant term `c` using methods like Lagrange interpolation or Gauss elimination.
4. Detecting incorrect points in the second test case.

### Input Format:
```json
{
    "keys": {
        "n": 4,
        "k": 3
    },
    "1": {
        "base": "10",
        "value": "4"
    },
    "2": {
        "base": "2",
        "value": "111"
    },
    "3": {
        "base": "10",
        "value": "12"
    },
    "6": {
        "base": "4",
        "value": "213"
    }
}

### 2ND Test Case:
{
    "keys": {
        "n": 9,
        "k": 6
    },
    "1": {
        "base": "10",
        "value": "28735619723837"
    },
    "2": {
        "base": "16",
        "value": "1A228867F0CA"
    },
    "3": {
        "base": "12",
        "value": "32811A4AA0B7B"
    },
    "4": {
        "base": "11",
        "value": "917978721331A"
    },
    "5": {
        "base": "16",
        "value": "1A22886782E1"
    },
    "6": {
        "base": "10",
        "value": "28735619654702"
    },
    "7": {
        "base": "14",
        "value": "71AB5070CC4B"
    },
    "8": {
        "base": "9",
        "value": "122662581541670"
    },
    "9": {
        "base": "8",
        "value": "642121030037605"
    }
}
​
