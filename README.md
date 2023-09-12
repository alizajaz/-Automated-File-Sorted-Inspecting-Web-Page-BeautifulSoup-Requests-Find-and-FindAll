# Automated-File-Sorter-in-File-Explorer-Python
This is basically moving different file types such as .csv,ong, jpg etc to the right folder path.
import os, shutil
path=r""#pathdirectory
file_name = os.listdir(path)#showpath
os.path.exist(path+'csv files')#checkfolder
folder_names=['csv files,'image files','text files']
for loop in range(0,3):
  if not os.path.exist(path + folder_names[loop])
              #print(path + folder_names[loop]))
        os.makedirs(path +folder_names[loop])

for file in file_name:
    if ".csv" in file and not  os.path.exist(path + "csv files/"+ file)
       shutil.move(path + file, path +"csv files/"+ file)#movefile
    elif ".png" in file and not  os.path.exist(path + "image files/"+ file)
       shutil.move(path + file, path +"image files/"+ file)#movefile
    elif ".txt" in file and not  os.path.exist(path + "csv files/"+ file)
       shutil.move(path + file, path +"text files/"+ file)#movefile
    else 
        print("There are files in this path were not moved!")
