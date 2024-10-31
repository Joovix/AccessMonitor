AccessMonitor
AccessMonitor é uma aplicação Python para monitoramento e gerenciamento de acessos remotos através do AnyDesk. Ele permite capturar, armazenar e gerenciar logs de conexão, oferecendo uma interface gráfica (GUI) e integração com Firebase para persistência de dados.

Índice
Funcionalidades
Instalação
Configuração do Firebase
Uso
Termos de Uso e Licença
Funcionalidades
Monitoramento em Tempo Real: Captura logs do AnyDesk continuamente.
Armazenamento e Sincronização com Firebase: Salva dados de acessos para persistência.
Resolução de Duplicidade de Nomes: Permite gerenciar IDs remotos duplicados.
Ocultar e Ignorar Acessos: Possibilidade de ocultar e ignorar determinados IDs na interface.
Abertura de Sessão AnyDesk Direto da Interface: Conexão rápida ao AnyDesk com um ID inserido.
Instalação
Pré-requisitos
Python 3.x
Bibliotecas Python: Instale com o seguinte comando:
bash
Copiar código
pip install firebase-admin tk
Clonando o Repositório
Clone o repositório do projeto:

bash
Copiar código
git clone <https://github.com/Joovix/AccessMonitor>
Executando a Aplicação
Navegue até o diretório do projeto e execute o script principal:

bash
Copiar código
python interface/main.py
Configuração do Firebase
Criação do Projeto no Firebase: Acesse o console do Firebase e crie um projeto.
Configuração de Credenciais: Baixe o arquivo de credenciais JSON do Firebase e salve-o no diretório interface/ com o nome acesso-anydesk-firebase-adminsdk-a2j5r-617aebce54.json.
Configuração de Regras: No Firebase, configure as permissões de leitura e escrita para a coleção acessos.
Uso
1. Interface Gráfica
Monitoramento de Acessos: Exibe uma lista de IDs remotos e permite nomeá-los.
Ocultar e Ignorar IDs: Para acessar, selecione um ID e escolha a ação “Ignorar” ou “Ocultar”.
Abrir Sessão AnyDesk: Insira um ID e clique em “Abrir AnyDesk” para iniciar uma conexão.
2. Resolução de Duplicidade
Se um nome já estiver em uso para outro ID, uma janela aparecerá solicitando um novo nome ou a opção de renomear o ID duplicado.
3. Logs e Erros
Todos os erros são registrados em logs/error_log.log para fácil consulta e depuração.
Termos de Uso e Licença
Este projeto está regido pelos seguintes documentos:

Termos de Uso
Licença MIT