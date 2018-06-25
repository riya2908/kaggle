import random
from matplotlib import pyplot as plt
from learntools.python.quickdraw import random_category, sample_images_of_category, draw_images_on_subplots

## Step 1: Sample some sketches
# How many sketches to view - a random number from 2 to 20
n = random.randint(2, 20)
# Choose a random quickdraw category. (Check out https://quickdraw.withgoogle.com/data for an overview of categories)
#print(n)
#n = 17
category = random_category()
imgs = sample_images_of_category(n, category)

## Step 2: Choose the grid properties
######## Your changes should go here ###############
if n<4:
    rows = (n+4)//4
    cols = min(n,4)
elif n%4==0 or (n<=8 and n>=4):
    rows = n//4
    cols = n//rows
else:
    rows=n//4
    cols=(n//rows) + 1
# The height and width of the whole grid, measured in inches.
height = rows * 2
width = cols * 2

## Step 3: Create the grid
grid = plt.subplots(rows, cols, figsize=(width, height))

## Step 4: Draw the sketches in the grid
draw_images_on_subplots(imgs, grid)
