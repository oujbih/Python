## save response to text 
```
import requests
response = requests.post("https://pdftables.com/api?&format=xlsx-single",files=files)
file = open("resp_text.txt", "w")
file.write(response.text)
file.close()
```
