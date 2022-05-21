#parent class
class User():
	
    def __init__(self, name, age, gender):      #constructor create
        self.name = name
        self.age = age
        self.gender = gender

    def show_details(self): 	#method,define function for next use
        print("Personal Details")
        print("")
        print("Name ", self.name)
        print("Age  ", self.age)
        print("Gender ", self.gender)

#child class
class Bank(User):
    def __init__(self, name, age, gender):		#useer define function  next use
        super().__init__(name, age, gender)
        self.balance = 0

    def deposit(self, amount):		#define function for deposit
        self.amount = amount
        self.balance = self.balance + self.amount
        print("Account balance has been updated : ", self.balance)

    def withdraw(self, amount):		#define function and money withraw condition.
        self.amount = amount
        if self.amount > self.balance:
            print("Insufficient Funds | Balance Available : ", self.balance)
        else:
            self.balance = self.balance - self.amount
            print("Account balance has been updated : ", self.balance )

    def view_balance(self): 	#define function for view balanc
        print("Account balance: ", self.balance)

ch1='y'
while(ch1=='y'):	#for repeat agein this code

    print("1. Create account")
    print("2. Diposit Money")
    print("3. Withraw money")
    print("4. Cheak balance")

    ch=int(input("Select any option : ")) #input 1-4 for option choise
    if(ch==1):
    	
    	#object create and input from user.
        n = Bank(input("Enter name :"),input("Enter age:"),input("Enter gender :" ))
        print("You have succefully crteated your bank acccount.")
    elif(ch==2):
        n.deposit(int(input("Enter the amount : ")))
    elif(ch==3):
        n.withdraw(int(input("Enter the withraw amount : ")))
    elif(ch==4):
        n.view_balance()

    else:
        print("please enter the right number.")
    print("Do you want to continue.....press y Button")
    ch1=input()





