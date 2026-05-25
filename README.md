# desafio-dio-pag-web
Projeto de site estático da Clínica Konoha com navegação entre páginas, formulário de contato, horário de atendimento e identidade visual inspirada no universo de Naruto.

Arquivos principais:
- `index.html`
- `about.html`
- `schedule.html`
- `contact.html`
- `base.css`
- `midia/96180-naruto-anime-hd-4k-5k-8k-logo.jpg`

Como executar localmente:

```bash
cd /home/wcsoliveira/projetos-web/desafio-dio-pag-web
python3 -m http.server 8000
```

Abra `http://localhost:8000` no navegador.

Painel (dashboard) lateral:

- A barra lateral foi transformada em um painel temático com botão de alternância (toggle).
- O botão tem a classe `menu-toggle`. Clicando nele a barra alterna entre o estado padrão e o estado compacto (colapsado).
- O estado colapsado é persistido no `localStorage` do navegador usando a chave `konoha:menuCollapsed`.
- Para forçar o menu a aparecer expandido, limpe o item do `localStorage` no console do navegador:

```js
localStorage.removeItem('konoha:menuCollapsed')
location.reload()
```

Notas sobre imagens:

- O projeto inclui uma imagem em `midia/96180-naruto-anime-hd-4k-5k-8k-logo.jpg`. Verifique direitos de uso antes de publicar publicamente.

O que foi melhorado:

- Navegação lateral com estilo de dashboard e ícones.
- Menu colapsável com persistência de estado entre visitas.
- Metadados `description` adicionados nas páginas para SEO básico.
- Herói com imagem temática e refinamentos de estilo em `base.css`.

Se quiser, eu posso gerar capturas das páginas ou empacotar o site em um arquivo `.zip` para distribuição.
