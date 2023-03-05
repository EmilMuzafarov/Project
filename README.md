num=input("Enter a number of seconds: ")
num=int(num)
display=input("Choose display type 1, 2, or 3: ")
display=int(display)
hours=num/3600
hours=int(hours)
mins=(num-hours*3600)/60
mins=int(mins)
secs=(num-hours*3600-mins*60)
secs=int(secs)
if (display==1):
  print(str(hours)+"h, "+str(mins)+"m, "+str(secs)+"s")
if (display==2):
  if (hours==1):
    print(str(hours)+" hour")
  else:
    print(str(hours)+" hours")
  if (mins==1):
    print(str(mins)+" minute")
  else:
    print(str(mins)+" minutes")
  if (secs==1):
    print(str(secs)+" second")
  else:
    print(str(secs)+" seconds")
if (display==3):
  if (hours<10):
    hours=("0"+str(hours))
  if (mins<10):
    mins=("0"+str(mins))
  if (secs<10):
    secs=("0"+str(secs))
  print(str(hours)+":"+str(mins)+":"+str(secs))# Project
