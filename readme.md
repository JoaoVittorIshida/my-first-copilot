# 🧩 Modos do Copiloto (Agent, Ask, Plan e Study)

![dio/me](https://img.shields.io/badge/dio-me-ff2d55)
![IA](https://img.shields.io/badge/IA-Assistente%20Inteligente-blue)
![Prompt](https://img.shields.io/badge/Prompt-engineering-yellow)

O Copiloto oferece uma suíte de **quatro modos de interação** otimizados para atuar com a persona "Cortana" (direta, calma e técnica). Você pode escolher como quer trabalhar: desde **tirar dúvidas sem o risco de alterar o código**, até **planejar arquiteturas complexas**, **delegar a escrita de features inteiras** ou **estudar novos conceitos a fundo**. 

A ideia é simples: selecione o modo que melhor combina com seu objetivo no momento e ganha velocidade com previsibilidade e controle absoluto sobre o seu projeto.

---

# 🤖 Agent Code
O **Agent Code** é o seu parceiro de execução. Sua missão é transformar requisitos em código limpo e implementável. Ele segue um ciclo rigoroso de **(A) Descobrir, (P) Planejar, (I) Implementar, (V) Verificar e (F) Finalizar**.

* **Forte:** Respeita o código existente (Regra do Não-Toque), não alucina arquivos fora do escopo e sempre entrega os trechos com o caminho exato do arquivo comentado no topo.
* **Ideal para:** Criar a tela inicial do Nummo em Kotlin, escrever o script de automação para a sua extensão web ou gerar a lógica de conexão WiFi do ESP32.
* **Comportamento:** Pensa em edge cases antes de codar e encerra com perguntas rápidas para destravar a próxima etapa.

📄 **Prompt:** [prompts/prompt-agent.md](prompts/prompt-agent.md)

---

# ❓ Ask
O modo **Ask** é para diagnósticos ágeis, leitura e investigação, **estritamente sem alterar seu código**. Ele atua com uma forte mentalidade de Quality Assurance (QA).

* **Forte:** Vai direto à causa raiz do problema e propõe formas rápidas de validar o erro antes de sugerir qualquer solução.
* **Ideal para:** Investigar por que um form não está preenchendo corretamente na sua extensão, analisar uma stack trace no console do Node.js ou debugar falhas no monitor serial do Arduino.
* **Comportamento:** Proibido de gerar blocos enormes de código proativamente. Responde sempre no formato: Diagnóstico, Causa Raiz, Como Validar e Opções de Abordagem.

📄 **Prompt:** [prompts/prompt-ask.md](prompts/prompt-ask.md)

---

# 🧭 Plan
O modo **Plan** atua como um arquiteto de software. Ele serve para **pensar, prever riscos e estruturar os passos antes de escrever uma única linha de código**.

* **Forte:** Foca em arquitetura (Clean, MVVM, MVC), mapeamento de dependências e estratégia de testes de integração.
* **Ideal para:** Estruturar a arquitetura geral de um novo aplicativo de controle financeiro, planejar o esquema do banco de dados ou desenhar o fluxo de comunicação MQTT de um sistema de alarme IoT.
* **Comportamento:** Proibido de implementar. Gera apenas documentos esquemáticos contendo Escopo, Estratégia, Arquivos Afetados, Riscos e um plano passo a passo revisável.

📄 **Prompt:** [prompts/prompt-plan.md](prompts/prompt-plan.md)

---

# 📚 Study
O modo **Study** é a sua tutora técnica sênior. O foco aqui não é resolver um bug correndo, mas sim **construir o seu modelo mental** e garantir que você domine o fundamento por trás da ferramenta.

* **Forte:** Usa analogias precisas, vai do simples ao avançado dependendo do seu nível e aplica checkpoints ativos para testar o que você absorveu.
* **Ideal para:** Entender a fundo como funciona o ciclo de vida de uma Activity no Android, dominar conceitos de Inteligência Artificial ou aprender boas práticas de concorrência e testes.
* **Comportamento:** Estrutura a resposta dividindo entre A Intuição do Conceito, A Prática (código limpo) e os Trade-offs/Armadilhas arquiteturais.

📄 **Prompt:** [prompts/prompt-study.md](prompts/prompt-study.md)

---

# 🧠 Resumo mental rápido
* **Agent** → Vai lá e coda (com segurança). 
* **Ask** → Lê, investiga e diagnostica o problema. 
* **Plan** → Arquiteta e mapeia riscos antes de agir. 
* **Study** → Ensina o porquê das coisas.