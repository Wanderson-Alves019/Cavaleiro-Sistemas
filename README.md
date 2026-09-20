# Cavaleiro Sistemas — Standalone

Este pacote é um site estático independente, com imagens locais e Firebase via CDN.

```bash
python3 -m http.server 8080
```

Depois acesse http://localhost:8080.

No Firebase Console, habilite Google Authentication, crie o Firestore, publique `firestore.rules` e adicione `localhost` em Authorized domains.

O painel Admin aparece somente para `wa758833@gmail.com`. O site salva e-mail, nome público e moedas na coleção `users`.

O login Google precisa de um servidor HTTP local ou hospedagem web; abrir diretamente por `file://` pode impedir o popup OAuth por restrições do navegador.
