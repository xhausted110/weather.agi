Weather.agi originally by Lonnie Abelbeck. First commit is as received from Steve Gemeny with his modifications. Further modified to read back the time.

Usage:
```
exten => 8675309,1,Answer
        same => n,Set(CHANNEL(language)=joan)
        same => n,AGI(weather.agi,http://www.weather.gov/xml/current_obs/KJFK.xml)
        same => n,Hangup
```
