# NfsController — FiscalFlow

Aplicação estática para registrar notas fiscais e vincular comprovantes de pagamento, preparada para hospedagem no GitHub Pages.

## Publicar no GitHub Pages

1. No GitHub, crie um repositório chamado **NfsController**.
2. Se for usar o repositório público, não coloque nele PDFs reais, comprovantes, backups ou outros dados financeiros.
3. Extraia este ZIP no computador.
4. No repositório, use **Add file → Upload files** e envie `index.html`, `README.md` e `.nojekyll` (se presente). Alternativamente, envie os arquivos por Git.
5. Abra **Settings → Pages**.
6. Em **Build and deployment**, escolha **Deploy from a branch**.
7. Selecione a branch `main` e a pasta `/(root)`; salve.
8. Aguarde a publicação e abra o endereço mostrado na seção **Pages**.

## Primeiro acesso e uso

- Na primeira abertura, crie uma senha local com pelo menos 8 caracteres.
- Para cadastrar uma nota, anexe primeiro o comprovante de pagamento e depois o PDF da nota fiscal.
- Confira os campos reconhecidos automaticamente antes de salvar; a leitura depende do texto extraível do PDF. PDFs digitalizados como imagem podem exigir preenchimento manual.
- Use **Exportar backup** regularmente e guarde o arquivo JSON em um local seguro. Faça um backup antes de restaurar outro.

## Limitações importantes

- Esta é uma aplicação estática: o GitHub Pages hospeda os arquivos, mas não fornece servidor, sincronização, contas de usuário nem banco de dados remoto para este projeto.
- As notas, PDFs, comprovantes e a senha configurada ficam no armazenamento local do navegador e do computador em uso. Eles não acompanham você automaticamente para outro navegador ou dispositivo.
- O login local é uma barreira simples, não equivale a autenticação de servidor e não criptografa os documentos armazenados.
- Limpar os dados do navegador, trocar de perfil ou perder o dispositivo pode apagar os registros. Mantenha backups protegidos.
- A leitura automática de PDFs carrega PDF.js de uma CDN e precisa de conexão com a internet para carregar essa biblioteca.

## Arquivos

- `index.html` — aplicação completa (HTML, CSS e JavaScript).
- `README.md` — instruções de publicação e uso.
- `.nojekyll` — indica ao GitHub Pages para não processar o conteúdo com Jekyll.
