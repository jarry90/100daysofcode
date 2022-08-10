# 100 Days of Code #

### 1/100 - 2 Aug ###

I've started the #100DaysOfCode challenge! I'll be updating here and on my twitter - [jarry90](https://twitter.com/Jared_Cavalli). It may not be daily, but I'll be focusing on Python, Django, JS and maybe more. Randomly, today I followed @ania_kubow's flight widget tutorial.

### 2/100 - 3 Aug ###

Starting strong, but more of an admin and planning day today. Updated my GitHub profile, added my flight widget to GitHub and started planning my personal website which will be built on Django and hosted on AWS Elastic Beanstalk? or Lightsail?

### 3/100 - 4 Aug ###

Had a busy day at work and looking after the kids. Still managed to get in a quick JavaScript tutorial and looked into some interesting APIs on [Public APIs](http://publicapis.dev). The [Owen Wilson wow API](https://owen-wilson-wow-api.herokuapp.com/) has inspired me! I might try making a FRIENDS related API

### 4/100 - 8 Aug ###

I went away with the family, so I took the weekend off. Today I created this repository and readme for my #100DaysOfCode log. I also researched my FRIENDS API. And stated [Roman Numerals Decoder kata](https://www.codewars.com/kata/51b6249c4612257ac0000005) at [Codewars](https://www.codewars.com/). I need to work out how roman numerals work 🤔. I've been slack, but am getting real tomorrow!

### 5/100 - 9 Aug ###

I continued the roman numeral decoder kata in python... haven't fully worked out roman numerals yet - will finish tomorrow.

I watched a few YouTube videos;
[Make MEMORY GAME in JavaScript, HTML and CSS for your portfolio](https://www.youtube.com/watch?v=W1GKhapHBB4)
[Have you done these 4 THINGS?? - Getting a job as a Software Developer](https://www.youtube.com/watch?v=JxUDdUU6N6k)

My plan to hit it hard has failed, but something is something. Hopefully get more done tomorrow!

### 6/100 - 10 Aug ###

I finally had a proper chunk to time to think about this. I finally worked out how roman numerals work - if the letter value is more than the next letter you add the value to the total, and if its less than the next, you subtract it.

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

### 7/100 ###
