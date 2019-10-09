import sys
filename = sys.argv[1]
min = sys.argv[2]
max = sys.argv[3]
f = open(filename)
lines = f.readlines()
for line in lines[1:]:
    columns = line.split(',')
    price = int (columns[9])
    if price >= int(min) and price <= int(max):
        print (line)
#this is just a test