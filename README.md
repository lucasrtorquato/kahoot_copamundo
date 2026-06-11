# 🏆 Kahoot Copa do Mundo — Hub de Acesso

Página central para acessar os Kahoots de cada grupo de alunos.  
Hospedada no **GitHub Pages**, sem dependências externas.

---

## 📁 Estrutura do projeto

```
seu-repositorio/
└── index.html   ← única página do projeto
```

---

## 🚀 Como publicar no GitHub Pages

1. Crie um repositório no GitHub (pode ser público ou privado com Pages ativado)
2. Faça upload do `index.html` na raiz do repositório
3. Vá em **Settings → Pages**
4. Em **Branch**, selecione `main` e a pasta `/ (root)`
5. Clique em **Save**

Após alguns segundos, sua página estará disponível em:
```
https://seu-usuario.github.io/nome-do-repositorio
```

---

## ✏️ Como adicionar os links dos grupos

Abra o `index.html` e localize os botões. Substitua o `href="#"` de cada grupo pelo link entregue pelos alunos:

```html
<!-- Antes -->
<a class="btn" href="#" target="_blank" rel="noopener">

<!-- Depois -->
<a class="btn" href="https://link-do-grupo1.com" target="_blank" rel="noopener">
```

Repita para cada um dos 7 grupos e faça o commit. A página atualiza automaticamente.

---

## 🎨 Personalização

| O que mudar | Onde no código |
|---|---|
| Nome da página | Tag `<title>` e o `<h1>` |
| Subtítulo | Tag `<span>` dentro do `<h1>` |
| Rótulo dos botões (`Grupo 1`, etc.) | Elemento com a classe `.label` |
| Cor da barra de cada grupo | Variável `--accent` nos seletores `:nth-child()` |
| Texto do rodapé | Tag `<footer>` |

---

## 🌐 Compatibilidade

- Funciona em qualquer navegador moderno (Chrome, Firefox, Safari, Edge)
- Layout responsivo — se adapta a celular e tablet automaticamente
- Sem JavaScript, sem frameworks, sem instalações
