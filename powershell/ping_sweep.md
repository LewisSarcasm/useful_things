```ps1
1..20 | % {"192.168.1.$($_): $(Test-Connection -count 1 -comp 192.168.1.$($_) -quiet)"}
```

Credit: https://learn-powershell.net/2011/01/31/quick-hits-ping-sweep-one-liner/
