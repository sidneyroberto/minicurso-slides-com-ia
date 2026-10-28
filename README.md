# Tutorial Passo a Passo: Criação de Slides Automáticos com NotebookLM e Google Gemini

Este tutorial guia você pelo fluxo de trabalho (_workflow_) idealizado por João Ernani para criar apresentações de slides profissionais, 100% editáveis e imunes a alucinações de IA, combinando o **NotebookLM (Gemini Notebook)** e o **Google Gemini**.

Como exemplo prático deste tutorial, utilizamos como fontes de conhecimento os documentos técnicos em PDF da Embrapa sobre a cultura e o cultivo do feijão no Brasil (tais como `cnpaf-embapa-1975.pdf`, `CIRCTECNICA89.pdf`, `CulturaFeijaoCaupiBrasil.pdf` e `doc48.pdf`, disponíveis [aqui](https://drive.google.com/drive/folders/12QL3BlCgpUUFIueKyQxSWJtV0_6gxHdy?usp=drive_link)).

---

## 🎯 Por que utilizar esta combinação?

1. **NotebookLM**: Atua como o "cérebro técnico" ancorado estritamente nas suas fontes confiáveis (PDFs, documentos, planilhas), garantindo que nenhum dado seja inventado ou alucinado.
2. **Google Gemini**: Atua como o "designer de apresentações", transformando o roteiro estruturado pelo NotebookLM em um arquivo nativo e totalmente editável no **Google Slides**.

---

## 🛠️ Passo a Passo do Workflow

### Passo 1: Preparação e Upload das Fontes no NotebookLM

1. Acesse o **NotebookLM** e crie um **Novo Notebook**.
2. Nomeie o seu projeto (exemplo: `Slides - Cultivo de Feijão Embrapa`).
3. Adicione os seus documentos de referência. Para este exemplo, selecione os PDFs da Embrapa armazenados no seu computador ou Google Drive.
4. O NotebookLM fará o processamento inicial e a leitura analítica das fontes.

---

### Passo 2: Geração do Roteiro Estruturado no NotebookLM

No painel central de chat do NotebookLM, insira o prompt especializado fornecido abaixo. Ele instrui a IA a atuar como um especialista no tema e a gerar um roteiro slide por slide fundamentado exclusivamente nos documentos.

#### 📝 Prompt para o NotebookLM:

```markdown
Atue como especialista em Ciências Agrárias e comunicação científica. Analise os documentos da Embrapa disponibilizados neste notebook e elabore o roteiro completo de uma apresentação didática sobre o cultivo de feijão no Brasil.

**REGRA FUNDAMENTAL: utilize exclusivamente os documentos fornecidos.** Não pesquise na internet, não consulte fontes externas e não acrescente informações provenientes de conhecimentos gerais. Não invente dados, recomendações, citações ou referências. Se uma informação não estiver disponível, informe isso claramente.

Organize a apresentação em aproximadamente 20 a 30 slides, ajustando a quantidade à relevância e à abrangência dos documentos.

Para cada slide, apresente:

1. **Título:** curto e informativo.
2. **Objetivo:** o que o público deverá compreender.
3. **Conteúdo:** tópicos objetivos, adequados à apresentação visual.
4. **Notas do apresentador:** explicações didáticas e detalhadas para orientar a exposição oral.
5. **Sugestão visual:** fotografia, gráfico, tabela, diagrama ou outro recurso pertinente.
6. **Fontes:** título do documento e página, seção, tabela ou figura de origem, quando identificáveis.

Organize os temas em uma sequência lógica, contemplando os principais aspectos do cultivo abordados nas fontes, como importância econômica, características da cultura, cultivares, clima, solo, implantação, manejo, pragas, doenças, colheita e produtividade, conforme a disponibilidade de informações.

Evite excesso de texto nos slides. Utilize as notas para aprofundar as explicações. Preserve os valores, as unidades de medida e as ressalvas técnicas dos documentos.

Inclua slides de introdução, conclusão e referências bibliográficas. Não apresente afirmações técnicas sem respaldo documental nem generalize resultados além do que as fontes me permitem.

Antes de finalizar, confira a coerência da apresentação e a correspondência entre as informações e suas fontes.

**Entregue o roteiro completo, organizado slide por slide, pronto para ser utilizado na criação de uma apresentação editável.**
```

Após a resposta do NotebookLM, **copie todo o texto do roteiro gerado**.

---

### Passo 3: Geração da Apresentação Editável no Google Gemini

1. Abra o **Google Gemini**.
2. Certifique-se de que a extensão ou ferramenta de integração visual / Canvas / Google Slides está habilitada nas configurações do Gemini.
3. Cole o prompt de design visual abaixo e, **logo em seguida**, cole o roteiro completo extraído do NotebookLM.

#### 🎨 Prompt para o Google Gemini:

```markdown
Crie uma **apresentação nativa e editável no Google Slides**, utilizando exclusivamente o roteiro fornecido em anexo.

### 1. REGRAS OBRIGATÓRIAS

- Crie slides, não um site, aplicativo ou documento HTML.
- Não inclua notas do apresentador nos slides. Elas serão inseridas posteriormente.
- Não consulte fontes externas nem invente informações.
- Preserve os dados, as unidades de medida, as referências e as ressalvas técnicas.
- Mantenha os elementos editáveis sempre que possível.

### 2. PRIMEIRO SLIDE — CAPA

Inclua o título da apresentação e a identificação do autor:
**Prof. Sidney Sousa**  
sidney.sousa@ifms.edu.br

Crie uma capa profissional, visualmente atraente e relacionada à agricultura brasileira.

### 3. DESIGN E APROVEITAMENTO DO ESPAÇO

Utilize o formato widescreen 16:9 e desenvolva uma apresentação com qualidade visual profissional.
**Aproveite adequadamente toda a área útil dos slides, tanto horizontal quanto verticalmente.**
Evite concentrar títulos e conteúdos na parte superior, deixando grandes espaços vazios na metade inferior.

Distribua os elementos de maneira equilibrada, utilizando:

- Grades e alinhamentos consistentes.
- Margens adequadas.
- Blocos de conteúdo bem dimensionados.
- Imagens integradas ao texto.
- Gráficos, diagramas e tabelas quando pertinentes.
- Destaques visuais para informações importantes.

Varie os layouts conforme o assunto. Utilize composições com imagens laterais, fotografias em destaque, duas colunas, comparações visuais, diagramas e outros formatos apropriados.
Não aumente artificialmente o tamanho dos textos apenas para preencher espaços vazios. Prefira melhorar a composição visual.
Mantenha uma identidade visual consistente, com tons de verde, fundos claros, tipografia legível e aparência técnico-científica.

### 4. USO DE IMAGENS, GRÁFICOS E OUTROS RECURSOS VISUAIS

**Sempre que contribuir para a compreensão do conteúdo, priorize recursos visuais em vez de apresentar apenas listas de tópicos.**
Utilize, conforme a pertinência:

- Fotografias de lavouras, plantas, cultivares e práticas agrícolas.
- Ilustrações explicativas.
- Diagramas e fluxogramas.
- Gráficos para representar dados quantitativos disponíveis.
- Tabelas comparativas.
- Esquemas de processos.
- Ícones discretos para facilitar a leitura.

Priorize imagens originais dos documentos fornecidos, quando disponíveis e adequadas para reutilização. Caso não estejam acessíveis, utilize imagens ilustrativas pertinentes, desde que isso seja permitido pelo ambiente utilizado.
Não apresente imagens ilustrativas como registros reais de experimentos.
Crie gráficos somente com dados efetivamente presentes no roteiro. Não invente valores, estatísticas ou resultados para preencher espaços.
Preserve as fontes dos dados e os créditos das imagens quando aplicáveis.

### 5. CONTEÚDO CIENTÍFICO

Utilize somente as informações do roteiro aprovado.
Mantenha os slides objetivos, com textos curtos e mensagens principais claras. Preserve as informações scientificas essenciais, sem sobrecarregar a área visual.
Não elimine ressalvas importantes nem altere o significado das afirmações.
Mantenha as referências bibliográficas associadas aos respectivos conteúdos, de forma discreta e legível.

### 6. ÚLTIMO SLIDE — AGRADECIMENTO

Finalize a apresentação com um slide visualmente harmonioso contendo:
**Obrigado pela atenção!**
**Prof. Sidney Sousa**  
sidney.sousa@ifms.edu.br

Destaque o e-mail para facilitar o contato.

### 7. REVISÃO E ENTREGA

Antes de finalizar, verifique:

- Se o espaço dos slides foi bem aproveitado.
- Se os elementos estão distribuídos equilibradamente na vertical e na horizontal.
- Se há recursos visuais suficientes e pertinentes.
- Se existem grandes espaços vazios evitáveis.
- Se os textos permanecem legíveis.
- Se os dados e as referências foram preservados.
- Se a apresentação está editável.
- Se a capa e o encerramento contêm as informações solicitadas.

Entregue a apresentação no Google Slides ou disponibilize a opção de exportação para essa ferramenta. Não entregue HTML ou imagens estáticas como substitutos da apresentação editável.
```

---

### Passo 4: Exportação e Organização Final no Google Slides

1. Após o Gemini gerar a estrutura visual, clique em **Exportar para Apresentações** ou **Abrir Apresentação**.
2. O arquivo será aberto nativamente no **Google Slides**.
3. **Pulo do Gato (Notas do Apresentador)**: Copie o trecho de _"Notas do apresentador"_ referente a cada slide (gerado no Passo 2 pelo NotebookLM) e cole na área inferior de notas do Google Slides respectivo.
4. Na hora da exposição, acesse **Visualização do Apresentador** (_Presenter View_) para conduzir a palestra com apoio de um roteiro detalhado sem poluir o visual dos slides para o público.

---

💡 **Dica de Ouro**: Esse fluxo economiza horas de trabalho e garante apresentações tecnicamente impecáveis, com design profissional e conteúdo 100% ancorado nas suas pesquisas e documentos de referência.
