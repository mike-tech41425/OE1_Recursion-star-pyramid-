question = input("how many is the base star? ")
def pyramid(star, row=1):   
    if row > star:
        return
    ash = " " * (star - row)
    pen = " *" * row

    print (ash + pen)
    pyramid(star, row + 1)

pyramid(int(question))
print(f"done pyramid with {question} * base")
