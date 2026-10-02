# F Dois Engenharia — Site institucional

Site estático (HTML, CSS e JavaScript puro, sem build e sem backend) da **F Dois Engenharia**, engenharia e construção civil em Natal-RN.

## Estrutura

```
index.html          página única
css/style.css       estilos
js/main.js          dados editáveis (CFG), animações, menu, filtros e lightbox
favicon.svg
assets/img/         fotos (também usadas como reserva dos vídeos)
assets/video/       vídeos curtos de 6 s (capa, seções e projetos)
```

## Rodar localmente

Abra o `index.html` no navegador ou, na pasta do projeto:

```
python3 -m http.server 8000
```

e acesse http://localhost:8000.

## Publicar no GitHub Pages

1. Crie um repositório no GitHub e envie todos os arquivos desta pasta (arraste-os em *Add file > Upload files* ou use `git push`).
2. Em **Settings > Pages**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`.
3. Em alguns minutos o site fica em `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.

Os caminhos são relativos, então funcionam em subpasta. Para domínio próprio, use o campo *Custom domain* na mesma tela.

## Como editar

Tudo que muda com frequência está no objeto `CFG`, no topo de `js/main.js`: contatos, redes sociais, link das avaliações do Google, números, serviços, projetos, diferenciais e depoimento.

- **Trocar uma imagem ou vídeo:** substitua o arquivo em `assets/` mantendo o mesmo nome. As fotos dos cards têm 640x480 px; vídeos de projeto, 6 s, sem áudio.
- **Projetos:** a ordem da lista `projects` no `CFG` acompanha a lista `PH` (foto, posição e vídeo de cada card).

## Pendências antes de publicar para o cliente

1. Trocar o link das avaliações do Google e o do LinkedIn em `CFG` (hoje são links de busca).
2. As fotos e vídeos são de banco de imagens e não são obras da F Dois. Substituir por obras reais e confirmar os direitos de uso. Os cards já trazem o selo "Imagem ilustrativa".
3. As categorias Institucional e Infraestrutura ainda não têm projetos reais; o filtro mostra um aviso.
4. Informar o link oficial do Instagram, se for diferente do atual.

## Informações da empresa

R. Dr. Múcio Galvão, 426 - Tirol, Natal - RN, 59020-550 · (84) 3234-3390 · WhatsApp +55 84 98846-4244
