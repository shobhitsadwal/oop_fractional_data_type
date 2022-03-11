# oop_fractional_data_type
this is the OOPS fractional data type built by the special methods or the dunder methods 

```python

  
# how to create our own data type

# now this is the decimal datatype
class FractionMaker:
    def __init__(self,num,denom):
        self.denom=denom
        self.num=num

    # def __str__(self):print(f'{self.num/self.denom}')

    def __str__(self): return f"{self.num}/{self.denom}"

    def __add__(self, other):
        down=self.denom*other.denom
        upp=self.denom*other.num+self.num*other.denom

        return f'{upp}/{down}'


    def __sub__(self, other):
        down=self.denom*other.denom
        upp=self.denom*other.num-self.num*other.denom

        return f'{upp}/{down}'


obj=FractionMaker(90,76)
makejs=FractionMaker(5,5)

```
