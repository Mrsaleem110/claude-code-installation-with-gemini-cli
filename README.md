# Claude-code-installation-with-gemini
.
### yeah sab powershell run at administrator mein run krna h.
# step 1 
### Generate gemini api key from google ai studio.
# step 2
### Required tool install karen is command sa.
 ```npm install -g @anthropic-ai/claude-code @musistudio/claude-code-router```
# step 3 
### Folder create kren.
```mkdir $HOME/.claude-code-router```
```mkdir $HOME/.claude-code```
# step 4 
### config.json create kren window method k lia.
```notepad $HOME/.claude-code-router/config.json```
# step 5 jab note pad open ho to yeah paste kren remember api key mein ja k google api key dalen or save kr len.
# 
```
{
  "LOG": true,
  "LOG_LEVEL": "info",
  "HOST": "127.0.0.1",
  "PORT": 3456,
  "API_TIMEOUT_MS": 600000,
  "Providers": [
    {
      "name": "gemini",
      "api_base_url": "https://generativelanguage.googleapis.com/v1beta/models/",
      "api_key": "$GOOGLE_API_KEY",
      "models": [
        "gemini-2.5-flash",
        "gemini-2.0-flash"
      ],
      "transformer": {
        "use": ["gemini"]
      }
    }
  ],
  "Router": {
    "default": "gemini,gemini-2.5-flash",
    "background": "gemini,gemini-2.5-flash",
    "think": "gemini,gemini-2.5-flash",
    "longContext": "gemini,gemini-2.5-flash",
    "longContextThreshold": 60000
  }
}
```
# step 6
 ### yeah commad terminal mein likh kr is mein bhi apni api key paste kren yad rahen yeah step k bad powershell close krdena.
``` [System.Environment]::SetEnvironmentVariable('GOOGLE_API_KEY', 'YOUR_KEY_HERE', 'User')```
# step 7 again powershell open kr h run at administration krna h or yeah paste krna h confirmation k lia k api set howe k nahi.
```echo $env:GOOGLE_API_KEY```
# step 8 installation version confirm kr len.
``` claude -version ```
```ccr version```
``` echo $env:GOOGLE_API_KEY```
# step 9 
 ### daily work flow start kren.
``` ccr start```
# step 10 
# claude code open kren.
```ccr code```
