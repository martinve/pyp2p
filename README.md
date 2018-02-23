# P2P Implementatsioon Pythonis

## TODO/Tegevusplaan

### Lokaalsed serverid

- Võtta aluseks Pythoni default socketserver ja panna käima selle baasinstallatsioon fikseeritud
    - Saata sinna suvalist datat ja veenduda, et vastus on ootuspärane
- Tekitada nimekiri peeridest ja vaadata kuidas seda kõige paremini hallata
    - Loon tekstifaili peeridest, milles igal real on kirje ip:port
    - Et peeride nimekirju samas füüsilises arvutis mugavalt hallata, nimetan need peers-<server_port>.txt, niimoodi teab
        iga instance, millisest failist lugeda. 
    - Teen GET päringuid peeride nimekirjas olevate IP-de vastu - kui saan vastuseks 404, kustutan nimekirjast peeri ära
    - Realiseerin serveris päringu `/getpeers`
        - _Päring_: getpeers
        + _Vastus_: JSON nimekiri teadaolevatest peeridest.
        
    Päringu tulemusel lisan päringut tegeva serveri peeride nimekirja need kirjed mida seal varem ei olnud.     
        
         
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

