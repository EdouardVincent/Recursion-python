# Recursion-with-python




def s(n):
    return n+1

def   p(n):
    return n-1

def addition(a,b):
    if b==0:
        return a
    else :
        return addition(s(a), p(b))
def multiplication(a,b):
    if b==0:
        return 0
    else :
        return addition(a,multiplication(a, p(b)))

def soustraction(a,b):
    if b==0:
        return a
    else:
        return soustraction(p(a), p(b))

def factoriel(a):   
    if a == 0:
        return 1
    else :
        return multiplication(a,factoriel(p(a)))


    
def puissance(a,b) :
    if b==0:
        return 1
    else :
        return multiplication(puissance(multiplication(a,b),p(b)),b)
    
def division2(a, b) :
    if b==0 :
        return a
    else :
        return soustraction(division2(a,b), division2(a,p(b)))
    
