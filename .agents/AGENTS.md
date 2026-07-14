# Agent Rules para o Blog Esdehubem

- **Deploy Automático**: Sempre que você (agente) criar, modificar ou excluir qualquer arquivo no projeto (como escrever um novo post, adicionar imagens, alterar configurações), você deve **automaticamente** realizar o commit e push para o GitHub (`git add .`, `git commit -m "..."`, `git push`). Isso é necessário para garantir que o deploy do GitHub Pages seja acionado sempre que houver mudanças. Não espere o usuário pedir, faça o push logo após finalizar as edições.
