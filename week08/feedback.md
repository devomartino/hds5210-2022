# Notes on the Midterm

* _Correctness    (out of 40):_ 24
* _Good Practices (out of 10):_ 9
* _Docs / Testing (out of 10):_ 9

_Details on the grading criteria for the midterm can be found on [Canvas](https://canvas.slu.edu/courses/28045/rubrics/23671)._

Overall, nicely done.

All of your functions hardcode in the name of the data file as `DATA` though, rather than using the `file` parameter passed into the function. This means that your code won't work if we change the file name.  I deducted 1 point from _Correctness_ for this.




## Step 1
* Nice work. No additional comments.

## Step 2
* No. The code needed to actually look at the information in the file and find the matching information for the provided billing_code and service_code. I'm not able to award any points for this: deducted 10 from _Correctness_

## Step 3
For the notes below, I deducted 1 point from _Good Practices_:
* Rather than repeating the information from the `get_rate()` function here, it would have been better to call the `get_rate()` function and then do the adjustments.
* Your `else` condition doesn't make sense. Doing `None` doesn't actually return `None`. In the case of the billing/service code combination not being found, your code would fail.

## Step 4
For the notes below, I've deducted 5 points from _Correctness_
* Your function should have just used the file name inputs rather than hardcoding them as `DATA1=...` and `DATA2=...`
* The `key` you seem to create for month is actually the whole date rather than just the month part of it.
* I found the rest of your code here hard to follow, but you can tell from the output it produces that it isn't working correctly.
* This function doesn't have any tests included in the docstring. I deducted 1 point from _Docs / Testing_ for that.