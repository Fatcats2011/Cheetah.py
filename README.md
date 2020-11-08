# Cheetah.py
import image 

pic = image.FileImage("Cheetah.jpg")
win = image.ImageWin(883,700,"Assign3")

for x in range(0,883):
#middle thrid
    for y in range(233, 466):
        w = pic.getWidth()
        h = pic.getHeight()       
        p = pic.getPixel(x, y)
        g = p.getGreen()
        r = p.getRed()
        b = p.getBlue()
        
        if r > 0 and g > 0 and b > 0:
            p.setRed(255)
            p.setGreen(0)
            p.setBlue(0)
                
#bottom third 
    for y in range(467,700):
        w = pic.getWidth()
        h = pic.getHeight()       
        p = pic.getPixel(x, y)
        g = p.getGreen()
        r = p.getRed()
        b = p.getBlue()
            
        if r > 0 and g > 0 and b > 0:
            p.setRed(255)
            p.setGreen(0)
            p.setBlue(0)

win.save("Image_new3.jpg")
