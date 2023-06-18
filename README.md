# assgn-6


Assignment 1a)
import json
# Data to be written
dictionary =[{
  "name" : "afreen",
  "DOB":"19/04/2003",
   "height" : "5'0",
   "city" : "vijayawada",
   "state" : "AP"
},{
  "name" : "seeta",
  "DOB":"14/06/2002",
   "height" : "5'5",
   "city" : "vijayawada",
   "state" : "AP"
},{
  "name" : "amrit",
  "DOB":"19/01/2003",
   "height" : "5'6",
   "city" : "vijayawada",
   "state" : "AP"
},{
  "name" : "feroz khan",
  "DOB":"19/04/1999",
   "height" : "5'7",
   "city" : "vijayawada",
   "state" : "AP"
},{
  "name" : "jhanvi",
  "DOB":"03/06/2003",
   "height" : "5'3",
   "city" : "hyderabad",
   "state" : "Telangana"
}]
  
# Serializing json
json_object = json.dumps(dictionary, indent = 4)
print(json_object)



Assignment 1b)
import json
# Data to be written
dictionary =[{
"key": "RJ",
"name": "Rajasthan"
},
{
"key": "SK",
"name": "Sikkim"
},
{
"key": "TN",
"name": "Tamil Nadu"
},
{
"key": "TS",
"name": "Telangana"
},
{
"key": "TR",
"name": "Tripura"
},
{
"key": "UK",
"name": "Uttar Pradesh"
},
{
"key": "UP",
"name": "Uttarakhand"
}]
# Serializing json
json_object = json.dumps(dictionary, indent = 4)
print(json_object)


Assignment 2

  def print_info(self):
        print('Pet Information:')
        print('   Name:', self.name)
        print('   Age:', self.age)

class Dog(Pet):
    def __init__(self, name, age, breed):
        super().__init__(name, age) 
        self.breed = breed
    def print_info(self):
        super().print_info()
        print ('   Breed:', self.breed)

pet_name = input()
pet_age = int(input())
dog_name = input()
dog_age = int(input())
dog_breed = input()

pet = Pet(pet_name, pet_age)
pet.print_info()
dog = Dog(dog_name, dog_age, dog_breed)
dog.print_info()
