# react-template-minimal-app
Minimal React application. 

Podle React - Das umfassende Handbuch, strana 43


## Spustit
`npx http-server .`  
Pak otevřít http://127.0.0.1:8080

### HTTPS
Vygeneroval jsem certifikát a klíč:  
`openssl req -newkey rsa:2048 -new -nodes -x509 -days 3650 -keyout key.pem -out cert.pem`  

Při otázce "Common name" jsem uvedl "127.0.0.1".  
cert.pem přidej we Windows do certifikátů uživatele, do Důvěryhodných kořenových certifikátů.

Spustit: `npx http-server -S -C c:\users\ext91476\cert.pem --key c:\users\ext91476\key.pem .`
