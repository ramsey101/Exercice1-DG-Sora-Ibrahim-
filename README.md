 # Exercice 1  
temp = float (input ("Entrez la temperature de l 'eau : "))

if temp <= 0 :

    print ("Cette temperature correspond à de la glace")
elif temp < 100 and temp > 0 :

    print ("Cette temperature correspond à du liquide")
else :

    print ("Cette température correspond à de la vapeur")
    
    
    
# Exercice 2
temp = float (input("Entrez la temperature de l'eau : "))

isGlace = temp <= 0

isLiquide = (temp < 100 and temp > 0)

isVapeur = temp > 100

if (isGlace) :

   print ("Cette temperature correspond à de la glace")
   
if (isLiquide) :

    print ("Cette temperature correspond à du liquide")
    
if (isVapeur) :

    print ("Cette temperature correspond à de la vapeur")
    
    
    
# Exercice 3
a = int(input("Entrez votre nombre : "))

n = 1

Hn = 0

while Hn < a :

    n+=1
    
    Hn=Hn+1/n
    
print(n)




# Exercice 4
p = 0.9

r = 1

foncVariable = p**((r-1)/r)

foncBase = foncVariable

while foncBase >= foncVariable:

    foncBase = foncVariable
    
    r=r+1
    
    foncBase=p**((r-1)/r)
    
print (r-1)



# Exercice 5
age = int (input("Entrez votre age : "))

permis = int (input("Entrez le nom d'année de votre permis : "))

accident = int (input("Entrez le nombre d 'accident que vous avez fait : "))

assur = int (input("Entrez le nombre d'année que vous etes assuré : "))

cond1 = age >= 25

cond2 = permis >= 2

cond3 = assur > 5

if not (cond1) and not (cond2):

    if accident == 0 :
    
        situation = "Rouge"
        
    else :
    
        situation = "Refusé"
        
elif ((not(cond1) and cond2) or (cond1 and not (cond2))) :

    if accident == 0 :
    
        situation = "Orange"
        
    elif accident == 1 :
    
        situation = "Rouge"
        
    else :
    
        situation = "Refusé"
        
else :

    if accident == 0 :
    
        situation = "Vert"
        
    elif accident == 1 :
    
        situation = "Orange"
        
    elif accident == 2 :
    
        situation = "Rouge"
        
    else :
    
        situation = "Refusé"
        
if cond3 :

    if situation == "Rouge" :
    
        situation = "Orange"
        
    elif situation == "Orange" :
    
        situation = "Vert"
        
    elif situation == "Vert" :
    
        situation = "Bleu"
        
print("Votre situation est : ", situation)
