# Leetcode_Day20
# Day 20 — LeetCode 35: Search Insert Position

## Problem

Given a sorted array of distinct integers and a target value, return the index if the target is found. If it is not found, return the index where it should be inserted to maintain the sorted order.

## Approach

Used **Binary Search** to solve the problem efficiently.

* Start with two pointers: `low` and `high`.
* Find the middle index using:
  `mid = low + (high - low) / 2`
* If `nums[mid] == target`, return `mid`.
* If the target is smaller, search the left half.
* If the target is larger, search the right half.
* When the loop ends, `low` represents the correct insertion position.

## Key Concept

The important idea here is that because the array is already sorted, we don't need to check every element.

Binary Search keeps cutting the search space in half, making the solution much faster than a simple linear search.

## Complexity

* **Time Complexity:** `O(log n)`
* **Space Complexity:** `O(1)`

## What I Learned

Today's problem was a simple reminder that **the way we approach a problem matters as much as the solution itself**.

A sorted array gives us useful information. Instead of ignoring it and checking everything, we can use that information to make our solution more efficient.

## Language

**Java**
