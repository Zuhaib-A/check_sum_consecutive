def solution(a, m, k):
    checking=len(a)-m
    temp_four=[]
    counter=0
    for i in a[0:checking+1]:
        index = a.index(i)
        
        temp_four.extend(a[index:index+(m)])

        displayed_matches=[]
        matches=[]
        for x in temp_four:
            
            index = temp_four.index(x)
            for i in range(len(temp_four)-1):
                
                
                if (x + temp_four[i] == 10) and (i != index) and ((index, i) not in matches):
                    matches.append((index, i))
                    displayed_matches.append((temp_four[index], temp_four[i]))
                    counter=counter+1

        print(temp_four)
        if len(displayed_matches) != 0:
            
            print(displayed_matches)
            print("\n")
        else:
            print("\n")
            
        temp_four=[]
        
    print("There are " + str(counter) + " total pairs.")
    return counter


length=int(input("How long is the list of numbers to check?\n"))


m=int(input("How long should the list of consecutive numbers be within the main list?\n"))
while m > length:
    m=int(input("Please try again, it should be less than the length of the entire list:\n"))

a=[]
for i in range(0,length):
    if i == 0:
        temp=int(input("Please add the 1st number:\n"))
        a.append(temp)

    elif i == 1:
        temp=int(input("Please add the 2nd number:\n"))
        a.append(temp)

    elif i == 2:
        temp=int(input("Please add the 3rd number:\n"))
        a.append(temp)

    else:
        temp=int(input("Please add the " + str(i+1) + "th number:\n"))
        a.append(temp)

k=int(input("And what should be the sum of the pairs?\n"))

print("\nYour final list to be checked is the following:\n" + str(a) +"\n")

solution(a,m,k)
