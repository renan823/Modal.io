# Modal.io
<p align="justify">Modal.io é uma biblioteca que adiciona modais criativos ao seu projeto!</p>

## Importação
<p>Faça o download dos arquivos "modal.js" e "style.css", encontrados neste repositório, e coloque-os em seu projeto.</p>

```html
<link rel="stylesheet" href="path/to/style.css">
<script src="path/to/modal.js"></script>
```

## Docs

### Modal básico
* Qualquer modal, para ser criado, precisa dos parâmetros "dimensions" (devem ser passadas em uma lista, no formato "[width, height]",<br> 
ou omitidas com "[ ]"), "title", "text" e "button" (nessa ordem): 
    ```html 
    <script>
        const modal = new Modal([], {msg: "Hello"}, {msg: "Hello world!"}, {msg: "Click here", color: "blue"});
    </script>
    ```
* O modal básico também pode ser usado para criar um modal de sucesso/erro:
  ```html 
    <script>
        const success = new SuccessModal([], {msg: "Oh Yeah"}, {msg: "Success!"}, {msg: "Close"});
        const error = new ErrorModal([], {msg: "Oh no"}, {msg: "Error!"}, {msg: "Close"});
    </script>
    ```

### Variáveis
* Dimensions: 
    ```html 
      <script>
          const dimensions = [width, height] || [];
      </script>
    ```
    <p> O parâmetro "dimensions" pode receber os tamanhos desejados, ou, simplesmente, usar os tamanhos pré definidos pelo sistema <br> (width = 350, heigth = auto).
    </p>
    
* Title: 
    ```html 
      <script>
          const title = {msg: "Hi", color: "orange"};
      </script>
    ```
    <p> O parâmetro "title" recebe uma objeto Javascript, que contém os items "msg", que refere-se ao conteúdo do título, e "color", 
    que refere-se à cor do título ("color" pode ser omitido, assim a cor será, por padrão, preto).
    </p>
    
* Text: 
    ```html 
      <script>
          const text = {msg: "Hello World!", color: "yellow"};
      </script>
    ```
    <p> O parâmetro "text" recebe uma objeto Javascript, que contém os items "msg", que refere-se ao conteúdo do texto, e "color", 
    que refere-se à cor do texto ("color" pode ser omitido, assim a cor será, por padrão, preto).
    </p>
    
* Button: 
    ```html 
      <script>
          const button = {msg: "Clik me", color: "purple"};
      </script>
    ```
    <p> O parâmetro "button" recebe uma objeto Javascript, que contém os items "msg", que refere-se ao texto do botão, e "color", 
    que refere-se à cor de fundo do botão ("color" pode ser omitido, assim a cor será, por padrão, azul).
    </p>
    
  
## Próximos passos
* Adicionar CSS via JS (eliminar "style.css")
* Criar novos modais 
* Criar animações
  

