# Implement A Multiplication Table

Please read the following requirement:

I want to create a multiplication table. The input should be 2 integers specifying the start and the end of the table:

AC1: The start number must be smaller than or equal to the end number. Or the function will return `null`.

AC2: The start number and the end number can be any number in a range of 1 to 1000 (inclusive).

AC3: The output should be a string represents the multiplication table. Suppose that the start number is *2* and the end number is *4*, the output should be something like the following. Please note that all columns should be aligned properly.

```
2*2=4
2*3=6  3*3=9
2*4=8  3*4=12  4*4=16
```

## Acceptance Criteria

* Please draw task diagrams.
* Please define all the methods according to your task diagram.
* Please write down a test case using *given...when...then* pattern for a leaf block. Then implement the block to pass the test.
* Please continue doing this work until all the requirement has been fulfilled.,

Given: startNum, endNum
When: IsStartNumLessThanOrEqualEndNum (startNum,endNum)
Then: Boolean must be returned (if start number is really less than or equal end number)

Given: startNum(equal to endNum), endNum
When: IsStartNumLessThanOrEqualEndNum (startNum,endNum)
Then: Boolean must be returned (if start number is really less than or equal end number)

Given: startNum(greater than endNum), endNum
When: IsStartNumLessThanOrEqualEndNum (startNum,endNum)
Then: false must be returned since start number is greater than end number.

Given: startNum, endNum
When: IsStartNumAndEndNumBetweenRange (startNum, endNum)
Then: Boolean must be returned (if startNum and endNum really is in between the range)

Given: startNum, endNum (above range)
When: IsStartNumAndEndNumBetweenRange (startNum, endNum)
Then: false must be returned since end number is above range

Given: startNum(less than range), endNum
When: IsStartNumAndEndNumBetweenRange (startNum, endNum)
Then: false must be returned since start number is less than range

Given: startNum(greater than endNum), endNum
When: CreateMultiplyTable (startNum, endNum)
Then: null must be returned since startNum is greater than endNum


Given: startNum(not within range), endNum
When: CreateMultiplyTable (startNum, endNum)
Then: "Start Number or End Number not within 1 to 1000" message must be prompted since start number is not within the range

Given: startNum, endNum
When: CreateMultiplyTable (startNum, endNum)
Then: a String of multiply table must be returned
