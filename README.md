# Projeto WebSite

### Este projeto foi desenvolvido usando a linguagem Python e Django.

### É um Web Site tipo BLOG para registrar/informar evolução nos estudos da Faculdade.

### O próximo passo é implementar um Banco de Dados e fazer a integração com o WebSite.

1. O Site está hospedado na Vercel.
2. Ele possui uma página Home, Contact, About, layout e projects.
3. A arquitetura das pastas foram organizadas assim comforme a imagem abaixo.
4. Criei um workflow ci/cd
5. Fiz integração com o n8n - criando um fluxo de mensagem que será enviada para o canal assim que o workflow for acionado.

<div align="center"> </div>
  <p float="left">
    <img src="api/static/images/Screenshot 2023-08-15 at 17.37.09.png" width="200" />
  </p>

4. Eu usei o ambiente de desenvolvimento integrado(IDE do inglês Integrated Development Environment) para desenvolver e editar o código.
   a - Linguagem Python;
   b - O Flask;
   c - Django...
   No arquivo requirements.txt tem uma lista completa das tecnologias usadas no projeto.

5. Para usar o projeto, após o **_git clone_** será necessário instalar o Python3.

- instalar o Python `yarn add python3`
- instalar a biblioteca Flask `pip install Flask`
- Atualizar o pip ` python3.11 -m pip install --upgrade pip`

6. Para ativar o Virtual Venv use o comando.

```
source venv/bin/activate

```

- Não esquecer de desativar o venv. `deactive`

7. Este projeto ainda está em construção.🚧 A próxima implementação será um Banco de Dados e um integração com GitHub e Vercel para automatizar a futuras atualizações do WebSite.

8. Caso você deseje colaborar com o projeto, será uma grande alegria receber sua colaboração.

9. 🚧 - Projeto em Construção

10. WebSite em [Vercel](https://website-red-eight.vercel.app/) clique e deixe sua opinião.

## Setup

### Install dependencies
Use the following command to install all required Python packages:
```
python3 -m pip install -r requirements.txt
```

### Running tests
To run the tests locally, use:
```
PYTHONPATH=. pytest -v tests/
```
This command ensures the `api` module is correctly found.

### Continuous Integration

The project is configured with a GitHub Actions workflow (`.github/workflows/ci.yml`) that:
- Lints the Python code using flake8
- Runs the tests
- Builds the project
- Deploys automatically to Vercel on pushes to `main` branch

Make sure to set your `VERCEL_TOKEN` secret in GitHub for deployment.

