# 💅 Pesquisa de CSAT e NPS (Serverless)

Um sistema completo e automatizado de Pesquisa de Satisfação (CSAT e NPS) desenvolvido para um estúdio de Nail Design. O projeto resolve problemas de custos de hospedagem e bloqueios de comunicação entre domínios (CORS) utilizando a arquitetura Serverless do ecossistema Google.

## 🚀 O Problema
Sistemas tradicionais de formulários e pesquisas exigem hospedagem web, configuração de banco de dados e APIs externas, gerando custos mensais ou limitando funcionalidades em planos gratuitos. Além disso, conexões entre páginas externas e planilhas frequentemente sofrem bloqueios de segurança de navegador (CORS).

## 💡 A Solução
Construímos uma aplicação onde o Front-end (HTML/CSS/JS) e o Back-end (Google Apps Script) residem nativamente dentro da mesma instância do Google Workspace. 

### Principais Benefícios:
* **Custo Zero:** Hospedagem gratuita no próprio Google Apps Script (Web App).
* **Ausência de CORS:** A página utiliza o método nativo `google.script.run` para enviar dados de forma limpa e direta para o backend.
* **Banco de Dados Integrado:** As respostas e os leads (amigas indicadas pelas clientes) são tabulados automaticamente em abas separadas no Google Sheets.
* **Alertas Inteligentes:** Uma automação identifica notas baixas (detratoras) e dispara imediatamente um e-mail de alerta para a gestão do estúdio.
* **Interface Limpa e Responsiva:** Design elegante e focado na experiência do usuário em dispositivos móveis.

## 🛠️ Tecnologias Utilizadas
* **Front-end:** HTML5, CSS3, Vanilla JavaScript.
* **Back-end:** Google Apps Script (`.gs`).
* **Banco de Dados:** Google Sheets.
* **Automação de E-mail:** Google MailApp Service.

## 📂 Como Implementar
1. Crie uma nova planilha no Google Sheets.
2. Acesse `Extensões > Apps Script`.
3. Adicione o código de `backend.gs` no arquivo `Código.gs` padrão.
4. Crie um arquivo HTML chamado `index.html` e cole o código do front-end.
5. Execute a função `configurarPlanilha()` para estruturar as abas automaticamente.
6. Publique como **Web App** definindo acesso para "Qualquer pessoa".

---
*Projeto desenvolvido para otimização de processos e captação estruturada de feedback.*
