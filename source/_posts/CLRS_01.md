---
title: 《算法巩固》学习第一天
date: 2018-03-30 17:14:53
tags: 算法
---

自己走在前端的茫茫人海中已经两年多了， 最近发现自己算法功底不是很好，就听从高人指点迷津开始算法巩固大学基础的第一天

* 题目
	给定一个整数数列，找出其中和为特定值的那两个数。你可以假设每个输入都只会有一种答案，同样的元素不能被重用。
	
	实例：

	>给定 nums = [2, 7, 11, 15], target = 9
	>因为 nums[0] + nums[1] = 2 + 7 = 9
	>所以返回 [0, 1]

* 普通的方案 (1)

```javascript
	/**
	* @param {number[]} nums
	* @param {number} target
	* @return {number[]}
	*/
	var twoSum = function(nums, target) {
	let result = [];
		for (var i = 0; i < nums.length; i++) {
			for (var j = 0; j < nums.length; j++) {
				if (i !== j) {
					if (nums[i] + nums[j] === target) {
						test = [j, i]
					}
				}
			}
		}
		return test
	};
```