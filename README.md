# Place
Land is the foundation of a country
class Nationí:
def __init__(self,land:bool):
self.land=land
self.exists=False
self.status=""Unknowm"
def evaluate_existence (self):
if self.land:
self.exists=True
self.status="The nation stands strong on its land."
else:
self.exists=False
self.status="No land.No foundation.The nation cannot exist."
def report(self):
print("===Nation Status Report===")
print(f"Land present:(self land)")
print(f"Nation exists:(self.exists)")
print(f"Message:(self.status)")
---Test cases---
1:Nation with land 
mongolia=Nation(land=True)
mongolia.evaluate_existence()
mongolia.report()
print()
2:Nation without land
no_land_nation=Nation(land=false)
no_land_nation.evaluate_existence()

no_land_nation.report()
