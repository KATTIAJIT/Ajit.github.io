
#hello


#import cv2
from PIL import ImageGrab

uid ="Ajit"


    
cap = cv2.VideoCapture(0)        
while True:
    screenshot = ImageGrab.grab()
    #hello1(uid,screenshot.tobytes(),screenshot)
    ret,frame = cap.read()
    frame=cv2.resize(frame,(640,480))
    data = cv2.imencode('.jpg',frame)[1].tobytes()
    #hello(uid,data)
    #try:

