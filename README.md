# Sorteios da Kelly - Firebase novo configurado

Este pacote já está configurado para usar o projeto Firebase novo:

- projectId: sorteio-f5431
- Firestore em tempo real
- Dezenas e centenas em coleções separadas
- Bloqueio por WhatsApp por sorteio
- Bloqueio de número/dezena/centena com transação para evitar duas pessoas escolherem o mesmo número ao mesmo tempo

## Antes de publicar

1. No Firebase Console, entre em Firestore Database.
2. Crie o banco de dados, se ainda não criou.
3. Vá em Regras.
4. Cole o conteúdo do arquivo `firebase-rules.txt`.
5. Clique em Publicar.
6. Envie estes arquivos para a Vercel.

## Arquivos principais

- `/dezenas/index.html`: página de dezenas
- `/centenas/index.html`: página de centenas
- `/admin/index.html`: redireciona para dezenas/admin
- `/assets/app.js`: sistema com Firebase
- `/assets/style.css`: visual do site

## Observação importante

As regras atuais estão abertas para facilitar o funcionamento. Para uso profissional, o ideal é criar login de admin e regras mais seguras.
