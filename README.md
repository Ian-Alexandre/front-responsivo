# Como Deixar Seu Site Responsivo em HTML e CSS

![GitHub](https://img.shields.io/badge/Status-Concluído-brightgreen)
![GitHub](https://img.shields.io/badge/Licença-MIT-blue)

Bem-vindo ao guia completo para criar sites responsivos usando HTML e CSS! Este ebook foi criado para ajudar desenvolvedores iniciantes e intermediários a entenderem os conceitos fundamentais de design responsivo e aplicá-los em seus projetos.

## Sumário

1. [Introdução ao Design Responsivo](#introdução-ao-design-responsivo)
2. [Viewport Meta Tag](#viewport-meta-tag)
3. [Unidades Relativas](#unidades-relativas)
4. [Media Queries](#media-queries)
5. [Layouts Flexíveis](#layouts-flexíveis)
6. [Imagens Responsivas](#imagens-responsivas)
7. [Testando a Responsividade](#testando-a-responsividade)
8. [Conclusão](#conclusão)

## Introdução ao Design Responsivo

Design responsivo é uma abordagem de desenvolvimento web que faz com que as páginas da web se adaptem a diferentes tamanhos de tela, desde desktops até dispositivos móveis. Isso é essencial para garantir uma boa experiência do usuário, independentemente do dispositivo utilizado.

## Viewport Meta Tag

O primeiro passo para criar um site responsivo é adicionar a meta tag `viewport` no `<head>` do seu documento HTML. Isso garante que a página seja dimensionada corretamente em dispositivos móveis.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

## Unidades Relativas

Usar unidades relativas como `%`, `em`, `rem`, `vh`, e `vw` em vez de unidades fixas como `px` ajuda a criar layouts que se adaptam a diferentes tamanhos de tela.

### Exemplo:

```css
.container {
    width: 90%;
    margin: 0 auto;
    padding: 2em;
}
```

## Media Queries

Media queries são a espinha dorsal do design responsivo. Elas permitem aplicar estilos CSS específicos com base nas características do dispositivo, como largura da tela.

### Exemplo:

```css
@media (max-width: 768px) {
    .container {
        width: 100%;
        padding: 1em;
    }
}
```

## Layouts Flexíveis

Usar `Flexbox` e `Grid` CSS facilita a criação de layouts que se ajustam automaticamente ao espaço disponível.

### Exemplo com Flexbox:

```css
.container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}

.item {
    flex: 1 1 200px;
    margin: 10px;
}
```

### Exemplo com Grid:

```css
.container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 10px;
}
```

## Imagens Responsivas

Para garantir que as imagens se ajustem corretamente, use a propriedade `max-width` e a tag `<picture>` para fornecer diferentes versões de uma imagem.

### Exemplo:

```html
<img src="image.jpg" alt="Descrição da imagem" style="max-width: 100%; height: auto;">
```

### Exemplo com `<picture>`:

```html
<picture>
    <source media="(min-width: 768px)" srcset="large-image.jpg">
    <source media="(min-width: 480px)" srcset="medium-image.jpg">
    <img src="small-image.jpg" alt="Descrição da imagem">
</picture>
```

## Testando a Responsividade

Use ferramentas como o Chrome DevTools para testar a responsividade do seu site. Simule diferentes dispositivos e verifique como o layout se comporta.

### Passos para Testar:

1. Abra o Chrome DevTools (F12 ou Ctrl+Shift+I).
2. Clique no ícone de dispositivo móvel (Ctrl+Shift+M).
3. Escolha um dispositivo ou defina um tamanho de tela personalizado.
4. Navegue pelo site e observe o comportamento.

## Conclusão

Criar um site responsivo é essencial nos dias de hoje, onde os usuários acessam a web de uma variedade de dispositivos. Com as técnicas apresentadas neste ebook, você está pronto para desenvolver sites que oferecem uma excelente experiência em qualquer tela.

### Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

---

**Autor:** [Ian Alexandre](https://github.com/ian-alexandre)  
**Contribuições:** Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

---

Espero que este ebook tenha sido útil para você! Se tiver alguma dúvida ou sugestão, não hesite em entrar em contato.

**Bons estudos!** 🚀
