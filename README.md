# PLAGARISM_HELP
Tools to help you cheat


When cheating, ensure that your code is different enough from the ones I show here. The following tool:

https://pypi.org/project/pycode-similar/

Will help with that. It checks the similarity of your code against the one you are using. I've found that code which is >30% similar does not get discovered as being copied. 


Methods that will not work:

Linting, will not alter the structure, just the variables and shape

Swapping function location, this will fail every time and will cause the TA to check closer for plagarism. It is a well known tactic to use.

Methods that DO work:

Defining variables with excessive steps. Ie: 

replace:

for i in range(len(x)):
  
with:

p = int(len(x))

for i in range(p):


Changing == to "is" and != to "is not":

if x == 10 and y != 9:

  
with:

p = str(x)

j = str(y)

if p is "10" and j is not "9":

Function fragnentation:

Replacing one large function with multiple smaller ones is a good method and renders identification almost impossible. Use of this method will result in the code similarity dropping ~10% per modified function on average. NOTE: DO NOT USE WHEN FUNCTIONS ARE PROVIDED FOR YOU.

Example:

def how_2_pass(x):

  if some code:
    
    some other code
   
   else some code:
      
      some other code

Replace with:

def some_function(p):

  some code
 
def some_other_function(o):
  
  some other code
  
def how_to_pass(x):

  if some code:
    
    some_function(p)
   
   else some code:
    
    some_other_function(o)
    
