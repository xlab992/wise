lista: https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/lista.m3u

epg: https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/epg.xml

---

Queste liste utilizzano un proxy su HuggingFace, se non funzionano create voi un vostro proxy

link del Proxy: https://github.com/nzo66/tvproxy

in alternativa potete usare mediaflow-proxy

---

Se create voi un proxy allora dovete fare il Fork di questa repo e modificare lista.py (se volete anche i canali esteri usate il branche world)

cosa modificare:

1️⃣ sostituisci "https://nzo66-piccolotest.hf.space" con il vostro url di HuggingFace, Render o altro se fate self host

se usate mediaflow proxy dovete anche sostituire "/proxy/m3u?url=" con "/proxy/hls/manifest.m3u8?api_password=test123&d="

adesso avrete un nuovo link tipo questo "https://aiiwa-adwa.hf.space/proxy/hls/manifest.m3u8?api_password=test123&d="

mi raccomando di mettere la vostra password del mediaflow-proxy in "api_password=test123&d=" (sostituire "test123" con la vostra password)

da modificare anche nella riga 297 - "&header_user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/133.0.0.0 Safari/537.36&header_referer=https://ilovetoplay.xyz/&header_origin=https://ilovetoplay.xyz\n"

"header_" deve diventare "h_" quindi cosi'

"&h_user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/133.0.0.0 Safari/537.36&h_referer=https://ilovetoplay.xyz/&h_origin=https://ilovetoplay.xyz\n"

2️⃣ cercate questo link https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/epg.xml e modificare "nzo66/TV" con il nome del vostro github e nome del fork  

---

Adesso Potete avviare Github Action e far partire lo script 

ricorda di dare i permessi del repo a Github Action 

