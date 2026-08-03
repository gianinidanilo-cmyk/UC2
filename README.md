# 🎓 TDS_UC02 - Elaborar Documentação de Sistemas

[![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)](https://git-scm.com/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/)
[![Markdown](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white)](https://daringfireball.net/projects/markdown/)
[![AI_Agents](https://img.shields.io/badge/AI_Agents-FF6F61?style=for-the-badge&logo=openai&logoColor=white)](https://github.com/features/copilot)

Este repositório reúne todo o material didático, guias de nivelamento, apostilas práticas e artefatos de configuração de Inteligência Artificial referentes à **Unidade Curricular 02 (UC02)** do **Curso Técnico em Desenvolvimento de Sistemas (TDS)** do **SENAC**. 

O objetivo principal desta UC é qualificar o futuro desenvolvedor para registrar, catalogar, gerenciar e automatizar a documentação técnica e de utilização de softwares, capacitando-o para o trabalho colaborativo de TI em conformidade com as exigências do mercado real.

---

## 🎯 Visão Geral da UC02 (36 Horas)

### 📊 Indicadores de Competência
1. **Elabora roteiro de uso** do software de acordo com suas funcionalidades.
2. **Elabora o manual de utilização** do projeto de software desenvolvido conforme orientação técnica.
3. **Seleciona a ferramenta de documentação**, de acordo com o projeto de software desenvolvido.
4. **Armazena as informações** usando recursos local ou em nuvem, de acordo com o projeto.
5. **Implanta rotinas de documentação automatizadas**, considerando produtividade e integração com a equipe de trabalho.

---

## 📅 Histórico de Aulas e Roteiros Práticos

O repositório está subdividido em aulas contendo guias instrucionais avançados:

### 📁 [Aula 07 - Trabalho Colaborativo na Prática](./Aula%2007)
Focada em simular um ambiente corporativo de TI, integrando controle de versão (Git/GitHub) com a correção de bugs em pequenos scripts JavaScript e Node.js.
* **Competências**: Criação e isolamento de ambientes com branches (`fix/`), resolução de tickets em quadros Kanban (MS Planner), submissão de Pull Requests (PRs) e revisão de código por pares (*Code Review* e *Merge*).
* **Material Complementar**: 
  - **[Guia_Aluno_Aula07.md](./Aula%2007/Guia_Aluno_Aula07.md)**: Roteiro passo a passo da dinâmica de trabalho corporativo.
  - **[guia essencial git.pdf](./Aula%2007/guia%20essencial%20git.pdf)**: Guia condensado de referência para Git.

### 📁 [Aula 08 - Reforço Prático de Colaboração](./Aula%2008)
Focada em desenvolver "memória muscular" no fluxo de trabalho distribuído ou modelo de contribuição em projetos *Open Source*.
* **Competências**: Uso prático do recurso **Fork** para clonar repositórios de colegas em contas próprias, criação de múltiplas branches (`feature/`) para envio de melhorias isoladas e atuação como mantenedor analisando, sugerindo alterações e aprovando Pull Requests no seu próprio projeto (`meu-site-simples`).
* **Material Complementar**:
  - **[Guia_Aluno_Aula08.md](./Aula%2008/Guia_Aluno_Aula08.md)**: Passos essenciais para a realização de Forks, múltiplas branches e aprovação/rejeição de contribuições de terceiros.

### 📁 [Aula 09 - Inteligência Artificial na Escrita Técnica](./Aula%2009)
*Crash course* sobre o uso produtivo e crítico de assistentes de Inteligência Artificial (LLMs) no desenvolvimento de software.
* **Competências**: Compreensão da mecânica básica de LLMs e mitigação de alucinações; aplicação de Engenharia de Prompts (Persona, Contexto, Instruções, Exemplos *Few-shot*, Restrições e Delimitadores); uso de Engenharia de Contexto na IDE (utilizando assistentes integrados para documentar código existente); e configuração de comportamento e automações no repositório através de arquivos de regras do agente (`.cursorrules`, `.agent/rules.md`).
* **Material Complementar**:
  - **[Guia_Aluno_Aula09.md](./Aula%2009/Guia_Aluno_Aula09.md)**: Guia de prompts, análise crítica de respostas, ferramentas integradas e automações guiadas por IA.

---

## 📄 Guia de Nivelamento: Git e Terminal (Windows/PowerShell)

O arquivo **[Guia NivelamentoGit](./Guia%20NivelamentoGit)** resume as instruções necessárias para configurar seu ambiente de desenvolvimento local:

### ⚙️ Configuração Inicial e Identidade
1. Instalação do Git no terminal do Windows (modo Administrador):
   ```powershell
   winget install --id Git.Git -e --source winget
   ```
2. Configuração de identidade global (executada uma única vez):
   ```bash
   git config --global user.name "Seu Nome"
   git config --global user.email "seu-email@exemplo.com"
   ```

### 🐚 Atalhos de Navegação do Terminal
* `pwd`: Exibe o caminho do diretório atual.
* `ls`: Lista arquivos e subpastas do diretório atual.
* `cd [pasta]`: Acessa a pasta desejada.
* `cd ..`: Retorna uma pasta no nível hierárquico.
* `mkdir [pasta]`: Cria uma nova pasta.
* `ni [arquivo.ext]`: Cria um arquivo vazio (PowerShell).
* `clear`: Limpa as informações do console.

### 🔄 Ciclo de Trabalho Local
```bash
git status              # 1. Verifica arquivos alterados/não rastreados
git add .               # 2. Adiciona as mudanças ao palco de preparação (Stage)
git commit -m "Mensagem" # 3. Cria um checkpoint/versão rotulada localmente
git log                 # 4. Exibe a linha do tempo dos commits
```

---

## 🧠 Skill de IA Especializada: Agent_Git (Modelo DPG)

O repositório traz o arquivo **[Danilo_PGianini.md](./Danilo_PGianini.md)**, que especifica as diretrizes de comportamento para um assistente inteligente especializado em documentação técnica baseado na metodologia **DPG (Diagnostic Programming Grid)**.

### 🔍 Estrutura do Modelo DPG
A Skill divide-se em três etapas lógicas de processamento para garantir uma análise estritamente fundamentada no código, reduzindo alucinações:

1. **🔹 D (Data Extraction)**: Extrai a árvore de diretórios, identifica a stack tecnológica (Node, Python, Java, etc.) e localiza os arquivos de configuração de dependências e entry points.
2. **🔹 P (Processing)**: Processa e identifica a arquitetura do sistema (MVC, API REST), analisando a distribuição das responsabilidades de cada camada e os padrões de organização lógica.
3. **🔹 G (Generation)**: Gera a documentação final de forma técnica, objetiva e estruturada, cobrindo:
   - Visão Geral e Tecnologias
   - Arquitetura do Sistema
   - Fluxo de Dados e Estrutura de Código
   - Passos de Execução
   - Gerenciamento de Dependências
   - Estrutura de Testes
   - Pontos de Atenção (Gaps de código/bugs)
   - Sugestões de Melhorias

---

## 🚀 Como Utilizar Este Repositório

Se você deseja consultar os materiais de aula e guias práticos:
1. Clone o repositório localmente:
   ```bash
   git clone https://github.com/gianinidanilo-cmyk/TDS_UC02.git
   cd TDS_UC02
   ```
2. Navegue até as pastas `Aula 07`, `Aula 08` ou `Aula 09` para ler os roteiros de aula escritos em Markdown.
3. O arquivo `Danilo_PGianini.md` pode ser lido ou copiado para a raiz de novos projetos como manual de instrução do seu agente de documentação.

---
*Documentação de apoio elaborada a partir dos planos de aula e arquivos do repositório TDS_UC02 do aluno Danilo Gianini.*
