# pet3
**Python Pet College Level
main.py

#import classes

import customer
def main():
    #Variables
    name = ""
    address = ""
    phone_number = ""
    email = ""
    pet_name = ""
    pet_type = ""
    pet_age = 0
    invoice_number = 0
    charges = 0.0 

#get user input
    name = input("Enter customer name:")
    address = input("Enter customer address:")
    phone_number = input("Enter customer phone:")
    email = input("Enter customer email:")
    pet_name = input("Enter pet name:")
    pet_type = input("Enter pet type:")
    pet_age = int(input("Enter pet age:"))
    charges = float(input("Enter charges incurred:"))
    invoice_number = int(input("Enter invoice assigned invoice #:"))

#print invoice
    myPerson = customer.Person(name, address, phone_number, email)
    print("***Carol's Pet Services***")
    print("Name:", myPerson.get_name())
    print("Address:", myPerson.get_address())
    print("Phone:", myPerson.get_phone_number())
    print("Email:", myPerson.get_email())
    myPet = customer.Pet(pet_name, pet_type, pet_age)
    print("Pet Name:", myPet.get_pet_name())
    print("Pet Type:", myPet.get_pet_type())
    print("Pet Age:", myPet.get_pet_age())
    myInvoice = customer.Invoice(invoice_number)
    print("Invoice #: \nCharges: ", myInvoice.get_charges())

main()
          
