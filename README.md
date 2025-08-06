# Projeto WebSite de desenvolvimento durante o periodo da Faculdade

### Este projeto foi desenvolvido usando a linguagem Python e Django.

### É um Web Site tipo BLOG para registrar/informar evolução nos estudos da Faculdade.

### O próximos passos:

- [] implementar um Banco de Dados
- [] fazer a integração com o WebSite.
- [✅] criar uma pipeline 

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
- Linguagem Python
- O Flask - um Framework poderoso e flexível que facilita o desenvolvimento de aplicações web e APIs com a linguagem de programação Python
- O Django - um Framework Ele oferece uma estrutura completa para o desenvolvimento de aplicações web, incluindo funcionalidades como roteamento, modelagem de dados, templates e segurança.
  
   No arquivo requirements.txt tem uma lista completa das tecnologias usadas no projeto.

5. Para usar o projeto, após o **_git clone_** será necessário instalar o Python3.

- instalar o Python
  
```
yarn add python3
```

- instalar a biblioteca Flask

```
pip install Flask
```
  
- Atualizar o pip
  
``` 
python3.11 -m pip install --upgrade pip
```

6. Para criar e ativar o Virtual Venv use o comando.

```
python -m venv <nome_do_ambiente>

source venv/bin/activate

```

- Não esquecer de desativar o venv. `deactive`

7. Este projeto ainda está em construção.🚧 A próxima implementação será implementar um Banco de Dados e um integração com GitHub e Vercel para automatizar a futuras atualizações do WebSite.

8. Caso você deseje colaborar com o projeto, será uma grande alegria receber sua colaboração.

9. 🚧 - Projeto em Construção -

10. WebSite em [Vercel](https://website-red-eight.vercel.app/) clique e deixe sua opinião.

## Setup

### Instalar DependIencias 

Use o seguinte comando para instalar todos os pacotes Python necessários:

```
python3 -m pip install -r requirements.txt
```

### Rodar os testes

Para executar os testes localmente, use:

```
PYTHONPATH=. pytest -v tests/
```

Este comando garante que o módulo `api` seja encontrado corretamente.

### Integração Contínua

O projeto é configurado com um fluxo de trabalho do GitHub Actions(`.github/workflows/ci.yml`) que:

- Lints do código Python usando flake8
- Executa os testes
- Compila o projeto
- Implanta automaticamente no Vercel ao enviar para a branch `main`

Certifique-se de definir seu TOKEN `VERCEL_TOKEN` no GitHub para implantação.



