# 100 Days of Code #

### 1/100 ###

### 2/100 ###

### 3/100 ###

### 4/100 ###

### 5/100 ###

### 6/100 - 10 Aug ###

I finally had a proper chunck to time to think about this. I finally worked out how roman numerals work - if the letter value is more than the next letter you add the value to the total, and if its less than the next, you subtract it.

Here is the solution I came up with.

```
def solution(roman):
    nums = {'I': 1, 'V': 5, 'X': 10, 'L': 50, 'C': 100, 'D': 500, 'M': 1000}
    number = 0
    for ref, letter in enumerate(roman):
        try:
            if nums[letter] < nums[roman[ref+1]]:
                number = number - nums[letter]
            else:
                number = number + nums[letter]
        except IndexError:
            number = number + nums[letter]
    return number
```

Looking at the other solutions on codewars.com I'm actually thinking this is a more elegent solution than most. So I'm happy :)

### 6/100 ###
