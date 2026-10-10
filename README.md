# 🎬 Ficha de Análise Audiovisual para TCC

Aplicação web desenvolvida em arquivo único (`index.html`) com o objetivo de auxiliar pesquisadores e estudantes na catalogação, organização e fichamento de evidências científicas e qualitativas extraídas de mídias audiovisuais (como vídeos do YouTube).

---

## 🚀 Principais Funcionalidades

1. **Metadados Inteligentes (YouTube OEmbed)**:
   - Ao colar um link válido do YouTube no campo de URL, o sistema busca e preenche automaticamente o **Título da Mídia** e o **Canal / Autor**.
   - Botão minimalista integrado para abrir o vídeo diretamente em uma nova aba.
   - As informações da mídia auditada permanecem fixas até que um novo link seja inserido.

2. **Campos com Máscaras e Formatação Automática**:
   - **Data de Publicação**: Máscara automática no formato `dd/mm/aaaa`.
   - **Duração do Vídeo**: Inserção automática de referências temporais no formato `00h00m00s`.
   - **Minutagem (Início e Fim)**: Padrão temporal de legendas automáticas (`00:00:00`), inserindo os dois-pontos `:` automaticamente conforme os números são digitados.

3. **Histórico de Personagens da Sessão**:
   - Armazena dinamicamente os nomes dos personagens/entrevistados utilizados durante a sessão via `sessionStorage`.
   - Oferece sugestões de autocomplete ao digitar, mantendo o histórico ativo mesmo ao auditar novos links de vídeos e apagando automaticamente ao fechar o navegador ou a aba.

4. **Gestão de Eixos Transversais (Temas)**:
   - Botões interativos de marcação temática pré-definidos (*Visitas, Crianças, Alimentação, Trajetórias, Trabalho, Território*).
   - Opção para adicionar novos temas personalizados sob demanda.

5. **Registro e Listagem de Blocos de Evidência**:
   - Campos dedicados para **Trecho Transcrito / Citação** (área expandida) e **Análise / Ligação com o TCC**.
   - Visualização em tempo real dos blocos registrados com opções de exclusão individual.

6. **Persistência de Dados e Exportação**:
   - Salvamento automático local (`localStorage`) para evitar perdas de dados.
   - Prévia interativa do relatório consolidado em modal.
   - Exportação rápida e direta nos formatos **.DOCX**, **.TXT** e **.MD** (Markdown).

---

## 🛠️ Tecnologias Utilizadas

- **HTML5 / CSS3** (Estrutura e estilização)
- **Tailwind CSS** (Framework CSS utilitário carregado via CDN)
- **FontAwesome** (Biblioteca de ícones)
- **JavaScript Vanilla (ES6+)** (Lógica de máscaras, requisições oEmbed, manipulação de DOM e armazenamento local/sessão)

---

## 📦 Como Usar

1. Baixe ou copie o código fonte completo da aplicação em um único arquivo chamado `index.html`.
2. Dê um duplo clique no arquivo para abri-lo em qualquer navegador moderno (Google Chrome, Firefox, Edge, Safari).
3. Comece a preencher os metadados do vídeo, insira os blocos de evidência com suas respectivas minutagens e exporte seu relatório pronto para o TCC!