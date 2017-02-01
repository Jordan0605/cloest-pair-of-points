This project implemented "The closest pair of points" algorithm with three methods: brute force, divide and conquer, enhanced divid and conquer.
The proposal of this project are to practice coding ability and to compare three methods' cost.
The details of three methods are shown below:

brute force
  You need to input a file as argv[1], this file's format is the same as example.input.
  This method is using nested loop to calculate every pair of points to find out which is the closest.
  Time complexity is O(n^2).

divide and conquer
  You need to input a file as argv[1], this file's format is the same as example.input.
  The largest size of input file is 10^5.
  You can input any size to test speedup and scalability.
  This method is to sort by x-coordinate first.
  Then find the middle point and recursively compare left side, right side and 2d-strip.
  When calculating 2d-strip, we sort the points by y-coordinate then test whether any pair's distance is less than original.
  Time complexity is O(n logn).


enhanced divide and conquer
  You need to input a file as argv[1], this file's format is the same as example.input.
  The largest size of input file is 10^5.
  You can input any size to test speedup and scalability.
  This method is to sort whole points in order first (including x and y axises).
  As method 2, we recursively compare left, right and strip.
  But we did not sort by y axis this time.
  Time complexity is O(n logn).
