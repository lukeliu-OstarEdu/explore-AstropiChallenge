from mpl_toolkits import mplot3d
import matplotlib.pyplot as plt
#create fig with 8 inch x 8 inch
fig = plt.figure(figsize=(8, 8))
ax = fig.add_subplot(projection='3d')

#open data file
file1 = open('F:\\Home\\CodingTutorial\\astropi\\Final\\explorer\\data\\magnetic_one_round.csv')
#read files
Lines = file1.readlines()


def Convert(string):
## covert the string in line to a list [longitude, latitude, intensity]

    li = list(string.split(','))
    return li


new_list =[]
#every line is one point, plot all of lines
for line in Lines:

  line = line.rstrip()
  lineList = Convert(line)
  #plot one point with latitude, longitude, intensity
  ax.scatter3D(float(lineList[1]),float(lineList[0]),float(lineList[2]))


# ax.axes.set_xlim3d(left=-180, right=180) 
# ax.axes.set_ylim3d(bottom=-60, top=60) 
# ax.axes.set_zlim3d(bottom=0, top=70) 

#set lab  
ax.set_xlabel('Longitude')
ax.set_ylabel('Latitude')
ax.set_zlabel('Magnetic Intensity')

#display chart
plt.show()

