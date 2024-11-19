# Portfólio CSS

O repositório traz o códio CSS para estilizar o portifólio. Com o missão de trazer uma iterface responsiva, bem documentada e acessível, focando em boas práticas de desenvolvimento front-end.


## Documentação do Código CSS

### Estrutura Geral
O código segue uma estrutura modular, que utiliza classes específicas para permitir a reutilização e consistência no design. COM estilos globais, como `*` e `body`, foram configurados para proporcionar uma base para a continuidade do código.

#### Exemplo:
```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    background-color: #151515;
}
```

---

### Classes Reutilizáveis
O código utiliza classes reutilizáveis para simplificar estilos comuns e impedir duplicidade.

#### Exemplos:
- **Classe `.section-about`**:
  Organiza os elementos da seção "sobre".
  ```css
  .section-about {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      margin: 20px 0;
      text-align: center;
      color: #fcfcfc;
      font-family: 'Poppins', sans-serif;
      padding: 0 20px;
  }
  ```
- **Classe `.cta-contact`**:
  Estiliza botões e links de chamada para ação, implementando efeitos ao passar o mouse.
  ```css
  .cta-contact {
      color: #ffffff;
      font-weight: 600;
      text-decoration: none;
      padding: 15px;
  }

  .cta-contact:hover {
      color: #c6c6c6;
      transform: scale(1.1);
      transition: all 0.6s;
  }
  ```

---

### Acessibilidade
Os estilos foram aplicados com foco em acessibilidade:
- **Contraste**: As cores do texto e do fundo (ex.: branco e cinza no fundo escuro) garantem boa legibilidade.
- **Scroll suave**: Possibilita uma navegação mais suavizada para todos os usuários.
  ```css
  html {
      scroll-behavior: smooth;
  }
  ```
- **Elementos focáveis**: Estilos foram aplicados para facilitar a navegação por teclado:
  ```css
  textarea:focus, input:focus, select:focus {
      outline: none;
  }
  ```

---

### Performance
Para otimizar o desempenho:
- **Uso de estilos globais mínimos**: Apenas o necessário foi incluído no seletor universal `*` para evitar impacto na renderização.
- **Imagens responsivas**: O tamanho das imagens é ajustado dinamicamente, utilizando `width: auto` e `height: auto`.
  ```css
  img {
      width: 70%;
      height: auto;
      margin: 0 0 20px;
  }
  ```
---

### Contribuindo
Se encontrar algo que possa ser otimizado ou documentado melhor, fique à vontade para abrir uma _issue_ ou enviar um _pull request_.

---
