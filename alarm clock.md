```python
from datetime import datetime
```


```python
from playsound import playsound
```


```python
alarm_time=input("enter the time of alarm to be set:HH:MM:SS\n")
alarm_hour=alarm_time[0:2]
alarm_mins=alarm_time[3:5]
alarm_secs=alarm_time[6:8]
print("Setting up an alarm........")
while True:
    now=datetime.now()
    current_hour=now.strftime("%H")
    current_minute=now.strftime("%M")
    current_seconds=now.strftime("%S")
    if(alarm_hour==current_hour):
         if(alarm_mins==current_minute):
            if(alarm_secs==current_seconds):
                print("wake up")
                playsound("Stopwatch-sound-effect.mp3")
                break
    
```


```python
now = datetime.now()

current_time = now.strftime("%H:%M:%S")
print("Current Time =", current_time)
```

    Current Time = 21:48:07
    


```python

```
