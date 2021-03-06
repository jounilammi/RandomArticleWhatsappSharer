# RandomArticleWhatsappSharer (RAWS)
RAWS is a Python3 app that can be used to share random Wikipedia knowledge to a Whatsapp group or a contact periodically.
It's great for sharing a fact of the minute/hour/day for your friend(s).

**NOTE: The element that is used for selecting the message field in WhatsApp Web may change and therefore the software may become unusable. Should this happen, please raise an issue so that I know to repair the selector.**

### What it does:
  - Uses Chromedriver to drive WhatsApp web
  - Fetches a random Wikipedia article in either Finnish or English, parses the first paragraph from it and turn the HTML version to plain text with html2text python library
  - Fetches the contact or group by given keyword and sends the first paragraph with a link to the specified user
  - Repeats the action when desired, max speed ~10 articles / minute
  ---
### How to use it
- Install Chromedriver to your chrome version from http://chromedriver.chromium.org/downloads
- Install the needed python packages:
```sh
pip3 install selenium
pip3 install requests
pip3 install html2text
```
- Set up control variables, they are located in the beginning of the Python code
- get your phone ready for scanning the Whatsapp QR code and start the app
- The app saves the Chrome options and therefore your Whatsapp login. This means that you only need to scan the WhatsApp QR once. Please note that the loging without QR scan may take time, minimum recommended LOGIN_PERIOD_SECONDS is 20 seconds.
---
### What it isn't
- RAWS is at a "working prototype" stage. This means, that bugs are possible.
- Known bugs:  
-- wrongly-written Wikipedia pages are likely to get printed wrongly  
-- "meta" pages such as category pages don't always work  
- The app isn't totally command-line because the first-time whatsapp verification needs to be done via the GUI and the app uses GUI to operate
### What it is
- A great way to either annoy or cheer up your friends
- A great way to learn something new every day
- A good start to develop something else to be shared via WhatsApp using Python


  
  
  
  


