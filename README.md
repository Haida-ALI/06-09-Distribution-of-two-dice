#distribution of rolling 2 die and calculating total 1000 times
from random import randint

def distribution(rolls):
  nums = {
    2:0,
    3:0,
    4:0,
    5:0,
    6:0,
    7:0,
    8:0,
    9:0,
    10:0,
    11:0,
    12:0
  }

  for x in range(rolls):
    total = randint(1,6) + randint(1,6)
    nums[total] += 1

  for i in range(2,13):
    print(f'{i}: {nums[i]}')




nums = {
  2:0,
  3:0,
  4:0,
  5:0,
  6:0,
  7:0,
  8:0,
  9:0,
  10:0,
  11:0,
  12:0
}

for x in range(1000):
  total = randint(1,6) + randint(1,6)
  nums[total] += 1

for i in range(2,13):
  print(f'{i}: {nums[i]}')
