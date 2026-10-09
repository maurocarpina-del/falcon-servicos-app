# Aplicativo BC (CAEL)

Crie um aplicativo mobile responsivo para seguranças de incêndio registrarem rondas diárias em prédios. O app deve se conectar ao Supabase utilizando as tabelas existentes: 'locais_ronda' e 'registros_rondas'.

Requisitos das telas:

1. Tela Inicial / Login Simples: Um campo para o segurança digitar o seu nome antes de iniciar.

2. Tela de Leitor de QR Code: Um leitor de QR code utilizando a câmera do celular (ou um campo de texto simulando o código caso testem no computador, ex: 'PRD01-EXT-01').

3. Ao ler ou buscar o QR code, o app deve consultar a tabela 'locais_ronda' pelo campo 'qr_code_hash' e exibir qual é o prédio e o local (ex: 'Edifício Teste - Extintor Hall de Entrada').

4. Botões de Ação:

   - Botão Verde "Tudo OK" (registra status 'OK' na tabela 'registros_rondas').

   - Botão Vermelho "Relatar Anomalia" (abre um campo de texto obrigatório para descrever o problema e registra o status 'ANOMALIA' na tabela 'registros_rondas').

5. Tela de Histórico / Painel Simples: Uma aba ou botão onde eu possa ver os últimos registros enviados com nome do segurança, local, status e horário.

This project was built with [Lovable](https://lovable.dev).

**Live app**: https://round-spotter-app.lovable.app

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/005f61fe-cf94-4c7a-9756-c3dbec9fc6d7).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
