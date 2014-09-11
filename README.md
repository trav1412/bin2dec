# this program converts binary numbers to decimal

def bin2dec(num):
  # takes a binary number as an input and returns the binary equivalent
  # num is a string representing a binary number like "10101" 
  result = 0
  for index in range(len(num)): 
    digit = num[index]
  if digit == '1':
    result = result + pow(2,len(num)-index-1)
  return result
