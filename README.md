# only-finger-track
Go to the Finger Detection and Tracking directory.
Then, 

1. Run the code with command `python FingerDetection.py`
2. Put your parm over the green squares
3. Then, press `z` key to start tracking
4. Finish program with `Esc` key.

`pip install requirements.txt`

# remove underscore https://github.com/dhruvaop/only-finger-track/blob/ninjas/Finger%20Detection%20and%20Tracking/FingerDetection.py#L94 if you are using opencv version higher that 3.4 then you have to remove `_`   if you are using opencv lower than 3.4 so it will work

1. instead of ` _, cont, hierarchy = cv2.findContours(thresh, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)` use `cont, hierarchy = cv2.findContours(thresh, cv2.RETR_TREE,    cv2.CHAIN_APPROX_SIMPLE)[-2:]` or `cnts,  = cv2.findContours(Mask.copy(), cv2.RETR_EXTERNAL,`

# update 
numpy==1.21.2
matplotlib==3.4.3
opencv-python==3.4.8.29



# if this code doesn't works then check the latest version for `numpy`, `matplotlib`, `opencv-python`

# change `pip install requirements.txt` to `pip install -r requirements.txt` for linux `$ pip install -r requirements.txt --no-index --find-links file:///tmp/packages` 
