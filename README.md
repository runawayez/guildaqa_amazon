# Guilda QA - Robot Framework

## Configuração do Ambiente

Antes de começar a executar os testes, certifique-se de que você tenha o seguinte configurado:

- Python [com opção Path] (versão 3.11.5): `https://www.python.org/downloads/`
- Robot Framework (versão 6.1.1) `pip install robotframework`
- VSCode (versão 1.82.2): `https://code.visualstudio.com/download`
    - Robot Framework Language: `https://marketplace.visualstudio.com/items?itemName=robocorp.robotframework-lsp`
    - Dracula Official (opcional): `https://marketplace.visualstudio.com/items?itemName=dracula-theme.theme-dracula`
    - Material Icon Theme (opcional): `https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme`
    - Selenium Library `pip install --upgrade robotframework-seleniumlibrary`
- Chromedriver (versão 117): `https://googlechromelabs.github.io/chrome-for-testing/`
    - Extrair executável do chromedriver na pasta "Scripts" do Python, exemplo: `C:\Users\[seu-usuario]\AppData\Local\Programs\Python\Python311\Scripts`

## Instalação

1. Clone este repositório para o seu sistema: `git clone https://github.com/runawayez/guildaqa_amazon.git`
2. Clique em Generate Git Credentials e cole sua chave de acesso
3. Abra o repositório com Open Folder do Vscode

## Executando os Testes

Para executar os testes, siga estas etapas:

1. Abra o terminal: `Ctrl+Shift+'`
2. Execute por tag testes da suíte usando o comando de tag: `robot -d ./resultados -i [TAG DESEJADA] amazon_testes_gherkin_bdd.robot`
    2.1 Este comando faz com que todas as evidências permaneçam organizadas dentro da pasta /resultados
3. Caso queira rodar por Caso de Teste, utilize: `robot -d ./resultados -t "[TÍTULO DO CASO DE TESTE AQUI]" amazon_testes_gherkin_bdd.robot`
    3.1 Exemplo de caso específico: `robot -d ./resultados -t "Caso de Teste 04 - Remover Produto do Carrinho" amazon_testes_gherkin_bdd.robot`