# P2P Implementatsioon Pythonis

## TODO

### Lokaalsed serverid

- Võtta aluseks Pythoni default socketserver ja panna käima selle baasinstallatsioon mingile suvalisele pordile
- Tekitada nimekiri peeridest ja vaadata kuidas seda kõige paremini hallata
- Võtta urllib teek ja teha sellega GET/POST päringuid serveri vastu
- Kui erinevaid instanceid käima/seisma panna tekitada olukord, et peeride nimekiri uueneks
    - Siis jagada peeride nimekirja instancite vahel, et see oleks alati ajakohane



## TBC

- Panen instanced jooksma erinevatel masinatel samas võrgus ja veendun, et need omavahel suhtlevad


## Teegid ja tööriistad

Võimalik valik:

### Python
- Server: socketserver
- Päringute tegemiseks: urllib

### Java
- Server: sisseehitatud httpserver
- Päringute tegemiseks: HttpURLConnection

### Node
- Server: express
- Päringute tegemiseks: http pakett

