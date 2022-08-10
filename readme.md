# 100 Days of Code #

### 1/100 ###

### 6/100 ###

I finally had a proper chunck to time to think about this. I finally worked out how roman numerals work - if the letter value is more than the next letter you add the value to the total, and if its less than the next, you subtract it.

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
