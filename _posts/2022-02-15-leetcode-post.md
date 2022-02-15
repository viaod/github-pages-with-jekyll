---
title: "[Java] - Using Leetcode for the first time"
date: 2022-02-15
----

Good evening, everyone!

I was scrolling through instagram and I saw a video about developing your coding skills.
I won't get into the details of the video because it's hard to explain, but it was quite funny :)
Anyway, one thing they mentioned was doing 2 LeetCode problems a day; I've decided to try 
doing so from this point on.

I'm not sure how feasible 2 problems a day is, especially as I have quite a bit of uni work 
to do right now, but one a day will do for now. I'm not a wiz or anything, so I'll increase/decrease
the amount and/or frequency depending on my work load.

This post will detail my first ever LeetCode question (I'm giving you all the privilege lol).

I attempted an easy question called Two Sum - this was in the top interview question section.
I decided to attempt an easy question to ease myself into the LeetCode life and it was not too complicated.

The solution I came up with was a nested for loop, with a O(n^2) complexity. 

class Solution {
    public int[] twoSum(int[] nums, int target) {
        for (int i = 0; i < nums.length; i++ ){
            for (int k = 0; k < nums.length; k++){
                if (nums[i] + nums[k] == target && i != k){
                    return new int[] {i,k};
                }
            }
        }
        return new int[] {};
    }
} 

This is a sound solution, but in the future I may look at reducuing the time complexity for a more effieient solution.

