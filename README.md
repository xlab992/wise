dopo aver fatto il fork di questa repo,
per prima cosa modifica il file lista.py,
modificare url1, url2, url4 del codice 
mettendo il link del tuo mediaflow-proxy
prima del link raw di github, dopo di che 
modifica anche il link raw di github sostituendo 
"nzo66/TV" con il vostro nome e nome del repo,
quindi "nzo66" sustutuiscilo con il nuo nome github
e "TV" con il nome del repo (se cambiato),

un po' più in basso nella riga "lista = '#EXTM3U x-tvg-url="https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/epg.xml"\n' + lista"
sostituisci anche li il nome github

dopo aver fatto ciò usa github action per avviare lo script (ricorda anche di dare i permessi a github action, cercate un tutorial)

adesso basta usare lista.m3u su un qualsiasi player iptv