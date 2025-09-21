def expanded_form(num):
    
    s = str(num)
    n = len(s)
    
    terms = []
    
    for i,digit in enumerate(s):
        if digit != "0":
            place_value = int(digit) * (10 ** (n-1-i))
            terms.append(str(place_value))
            
    return " + ".join(terms)
