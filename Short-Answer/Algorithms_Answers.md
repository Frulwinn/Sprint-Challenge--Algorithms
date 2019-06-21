Add your answers to the Algorithms exercises here.
Exercise I

a) run time = O(n)
The run time is linear time because the number of additional operations the algorithm needs to perform grows in direct proportion to the increase in input size.

b) run time = O(n^4)
It's a nested loop so it requires multiple operations for input i, j, k, and l. When we add all the loops we get quadratic time.

c) run time = O(n)
With a base case of 0 this method will rund down till it reaches 0 so the algorithm decreases in direct proportion to the input size which makes it linear time.

Exercise II
This sounds like a good case for using binary search.

We have som given variables.
Building = _n_ story
_f_ = floor
Eggs break if thrown >= _f_
Eggs don't break if thrown <= _f_
Floors are sorted.

I would find the median '_f_' of the n story building.

Once I find the median '_f_' I would throw out an egg off that '_f_'. If it broke I would focus on the '_f_' below that median '_f_', making the initial median the new highest value for '_f_'.

Then I would find the new median of the new range and throw an egg off that '_f_'. If the egg breaks I would again focus on the '_f_' below that median value, make the median value the new highest value for '_f_'.

I would repeat this procedure until I find the '_f_' value where the egg does not break.

run time = O(log n)
This is the run time because the algorithm keeps breaking into half with each iteration until the value is found.