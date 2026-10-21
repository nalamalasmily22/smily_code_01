# smily_code_01# 1. Sort words and convert them to lowercase

with open("source.txt", "r") as file:
    words = file.read().lower().split()

words.sort()

with open("output.txt", "w") as file:
    file.write("\n".join(words))

print("Sorted lowercase words saved to output.txt")


# 2. Print each line in reverse order

with open("source.txt", "r") as file:
    lines = file.readlines()

print("\nEach line in reverse order:")

for line in lines:
    print(line.rstrip("\n")[::-1])
