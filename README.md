# myRaspiberryProject

This my first project with raspiberry pi. I am very exicited with what I was able accomplish here. 

## running locally
Make sure you have installed yagmail in your raspiberry, You will need 2 email addresses. One will be the sender and the other the receiver. In the main file you will need to put your email in the send_email_with_photo(yagmail_client, file_name) function.

```python
password = ""
with open("/home/pi/.local/share/.email_password", "r") as f:
    password = f.read()
yag = yagmail.SMTP("raspiberry@gmail.com", password)
print("Email sender setup OK.")
```
Here you will have to setup your password. In my case, I created a hidden file with my password to keep things private.
Now you will open 2 terminal windows in one window you will go to the code directory and then run the command `python3 main.py`. In the second window you will go to the code directory and run `python3 server.py`

If everything was setup correctly you should be able to test it.

you go check it on my youtube channel: [MY FIRST RASPIBERRY PI PROJECT](https://www.youtube.com/watch?v=ZeqKMSR4VPQ)
