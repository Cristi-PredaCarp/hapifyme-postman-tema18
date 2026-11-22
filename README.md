# Tema 18 - HTTP & Postman
Autor: Cristi Preda

Colecția automatizează ciclul de viață al unui utilizator hapifyMe:
1. Register — generează date unice și creează contul.
2. Confirm Email — confirmă contul.
3. Login — salvează JWT și ID-ul utilizatorului în Environment.
4. Get Profile — verifică emailul contului creat.
5. Delete Profile — șterge contul folosind Bearer Token.

## Rulare
1. Importă cele două fișiere JSON în Postman.
2. Selectează mediul HapifyMe Tema Env.
3. Deschide Collection Runner.
4. Rulează toate cele cinci cereri în ordinea de mai sus, cu o iterație.

Doar baseUrl este completat în mediul exportat.
Celelalte valori sunt generate sau extrase automat la rulare.

## Particularități API
Login folosește username-ul returnat la înregistrare.
Emailul generat este verificat în răspunsurile Login și Get Profile.
Get Profile folosește API key în headerul Authorization și user_id în query.
Delete Profile folosește JWT prin Bearer Token.

## Rezultat
Rulare verificată: 12 teste trecute, 0 eșuate.
