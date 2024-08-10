# index.html

## Descrição
Consiste em uma página web que permite aos usuários colar um link de vídeo do YouTube e exibir a thumbnail correspondente. A página é responsiva e projetada para funcionar em vários dispositivos.

## Métodos e Propriedades

- **document.getElementById('element_id')**:
    - **Descrição:** Método do DOM que retorna uma referência ao elemento com o ID especificado.
    - **Parâmetros:**
        - `'element_id'`: ID do elemento HTML a ser encontrado.

- **split()**:
    - **Descrição:** Método de string em JavaScript que divide uma string em um array de substrings com base em um separador.
    - **Parâmetros:**
        - `('v=')`: O separador usado para dividir a string.

- **setAttribute('attribute', 'value')**:
    - **Descrição:** Método do DOM que define o valor de um atributo em um elemento HTML.
    - **Parâmetros:**
        - `'attribute'`: Nome do atributo a ser definido.
        - `'value'`: Valor a ser atribuído ao atributo.

## Lógica

1. **Captura do Link do Vídeo:**
    - Ao clicar no botão "Get it now!", a função `get_thumbnail()` é chamada para obter o valor do link do vídeo inserido pelo usuário.

2. **Obtenção do ID do Vídeo:**
    - O ID do vídeo é extraído do link do YouTube utilizando a função `split('v=')[1]`.

3. **Exibição da Thumbnail:**
    - O ID do vídeo é incorporado em uma URL fixa para obter a thumbnail correspondente, que é então exibida na página.

## Funcionamento
- O usuário insere o link do vídeo do YouTube no campo de entrada.
- Após clicar no botão "Get it now!", a função JavaScript é acionada para extrair o ID do vídeo e exibir a thumbnail associada.

# site_1.py

## Descrição
O código apresentado é uma aplicação web simples usando o framework Flask em Python. A aplicação possui uma rota padrão ('/') que renderiza um template HTML chamado 'index.html'.

## Métodos e Propriedades

- **Flask()**: 
    - **Descrição:** Classe principal do Flask que representa a aplicação web.
    - **Propriedades:**
        - `__name__`: Propriedade que define o nome do módulo ou pacote da aplicação.
    - **Métodos:**
        - `route()`: Decorador usado para associar uma função a uma rota específica.

- **index()**: 
    - **Descrição:** Função que é executada quando a rota padrão ('/') é acessada.
    - **Retorno:** Renderiza o template HTML 'index.html'.

- **render_template()**: 
    - **Descrição:** Função do Flask utilizada para renderizar templates HTML.
    - **Parâmetros:**
        - Nome do template a ser renderizado.

- **app.run()**: 
    - **Descrição:** Método que inicia o servidor de desenvolvimento Flask.
    - **Parâmetros:**
        - `debug=True`: Habilita o modo de depuração, permitindo recarregar automaticamente o aplicativo quando o código é alterado.

## Lógica

1. **Inicialização do Flask:**
    - A aplicação Flask é inicializada com o nome do módulo atual.

2. **Rota '/' (index):**
    - Quando o usuário acessa a rota padrão ('/'), a função `index()` é acionada.
    - Essa função renderiza o template HTML 'index.html'.

3. **Execução do Aplicativo:**
    - O servidor de desenvolvimento Flask é iniciado apenas se o script for executado diretamente, não se for importado como módulo.
    - O modo de depuração é habilitado, permitindo recarregar automaticamente o aplicativo em caso de alterações no código.

## Funcionamento
- Quando o servidor Flask é iniciado, ele aguarda requisições dos clientes.
- Ao acessar a rota padrão ('/'), o conteúdo do arquivo 'index.html' é exibido no navegador.

Esta documentação fornece uma visão geral do código "Get Youtube Thumbnail", detalhando seus métodos, propriedades e a lógica por trás da funcionalidade de obtenção e exibição de thumbnails do YouTube.
