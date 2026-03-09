# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href="https://www.fiap.com.br/">
<img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Administração Paulista" border="0" width="40%" height="40%">
</a>
</p>

<br>

# CardioIA – Batimentos de Dados


## Integrantes

- Otávio Custódio — RM: 565606  
- Matheus Parra — RM: 561907  
- Tiago Alves Cordeiro — RM: 561791  
- Thiago Henrique Pereira de Almeida Santos — RM: 563327  
- Leandro Arthur Marinho Ferreira  

---


## 👩‍🏫 Professores

### Tutor
- Caique Nonato

### Coordenador
- Andre Godoi

---

# Introdução

Neste projeto assumimos o papel de cientistas de dados hospitalares com o objetivo de reunir, organizar e compreender diferentes tipos de dados relacionados à saúde cardiovascular.

Esses dados serão utilizados nas próximas fases do projeto **CardioIA**, alimentando algoritmos de Inteligência Artificial voltados para análise médica, apoio ao diagnóstico e identificação de padrões relacionados a doenças cardíacas.

O projeto também considera conceitos importantes de **Governança de Dados**, como qualidade, organização e possível presença de vieses nos dados.

---

# Parte 1 – Dados Numéricos (IoT)

Foi criado um dataset contendo informações simuladas de pacientes cardíacos.

O conjunto de dados possui mais de **100 registros** com variáveis relevantes para análise médica.

## Variáveis utilizadas

- idade
- sexo
- pressão arterial
- colesterol
- frequência cardíaca
- diabetes
- tabagismo
- nível de atividade física
- sintomas
- presença de doença cardíaca

## Origem dos dados

Os dados são **simulados com base em padrões médicos comuns descritos em literatura científica sobre fatores de risco cardiovasculares**, como idade avançada, pressão arterial elevada e colesterol alto.

Essa abordagem permite criar um conjunto de dados controlado para testes e desenvolvimento de modelos de IA.

## Variáveis mais relevantes para IA

Algumas variáveis possuem grande impacto na análise de risco cardiovascular:

**Pressão arterial:**  
Valores elevados estão diretamente relacionados ao risco de doenças cardíacas.

**Colesterol:**  
Altos níveis de colesterol aumentam a probabilidade de formação de placas nas artérias.

**Frequência cardíaca:**  
Alterações podem indicar problemas cardiovasculares ou estresse fisiológico.

**Idade:**  
O risco de doenças cardíacas aumenta com o envelhecimento.

Essas variáveis podem ser utilizadas por algoritmos de **Machine Learning** para prever a probabilidade de um paciente desenvolver problemas cardíacos.

---

# Parte 2 – Dados Textuais (NLP)

Foram coletados dois textos relacionados à saúde cardiovascular, sintomas e diagnóstico de doenças cardíacas.

Os arquivos estão disponíveis na pasta:

docs/


## Possíveis aplicações com NLP

Os textos podem ser utilizados em algoritmos de **Processamento de Linguagem Natural (NLP)** para diversas análises, como:

- Extração automática de sintomas
- Classificação de tópicos médicos
- Identificação de termos relacionados a doenças
- Análise de frequência de palavras relacionadas à saúde cardiovascular

## Importância para projetos de IA em saúde

A análise de textos médicos pode auxiliar no desenvolvimento de sistemas capazes de:

- analisar prontuários médicos
- identificar sintomas relatados por pacientes
- auxiliar médicos no diagnóstico clínico
- gerar insights a partir de grandes volumes de literatura médica

---

# Parte 3 – Dados Visuais (Visão Computacional)

Foram reunidas **mais de 100 imagens de eletrocardiogramas (ECG)**.

Essas imagens representam sinais elétricos do coração e são amplamente utilizadas para diagnóstico de diversas condições cardíacas.
## Estrutura das Imagens de ECG

As imagens de eletrocardiograma (ECG) foram organizadas em pastas que representam diferentes tipos de batimentos cardíacos. Essa organização segue o padrão utilizado em diversos datasets de pesquisa em cardiologia e aprendizado de máquina.

Estrutura das pastas:

assets/ecg_images  
├── N  
├── V  
├── S  
├── Q  
├── M  
└── F  

### Significado das Classes de Batimentos

| Pasta | Tipo de Batimento | Descrição |
|------|------------------|-----------|
| **N** | Normal | Batimento cardíaco normal, sem sinais aparentes de anomalia. |
| **V** | Ventricular | Batimento ventricular prematuro, associado a arritmias cardíacas. |
| **S** | Supraventricular | Batimentos originados acima dos ventrículos, podendo indicar irregularidades no ritmo cardíaco. |
| **F** | Fusional | Batimento resultante da fusão entre um batimento normal e um ventricular. |
| **Q** | Desconhecido | Batimentos que não puderam ser classificados com precisão. |
| **M** | Miscellaneous | Categoria que representa outros tipos de batimentos ou variações menos comuns. |

### Aplicação em Inteligência Artificial

A organização das imagens por tipo de batimento permite que algoritmos de **Visão Computacional** e **Deep Learning** sejam treinados para reconhecer padrões específicos em sinais cardíacos.

Esses modelos podem aprender a:

- identificar batimentos cardíacos anormais
- detectar arritmias
- classificar exames de ECG automaticamente
- auxiliar médicos no diagnóstico precoce de doenças cardiovasculares

Esse tipo de abordagem é amplamente utilizado em sistemas de apoio à decisão médica baseados em Inteligência Artificial.

## Aplicações com Visão Computacional

As imagens poderão ser analisadas por algoritmos de **Computer Vision** para:

- detecção de padrões anormais no ECG
- identificação de arritmias
- reconhecimento de irregularidades no ritmo cardíaco
- classificação de exames normais e anormais

## Importância para IA médica

A Visão Computacional aplicada à cardiologia permite desenvolver sistemas capazes de auxiliar médicos na análise automática de exames, reduzindo tempo de diagnóstico e aumentando a precisão na identificação de problemas cardíacos.

---

# Links para os dados completos

Os datasets completos estão hospedados no Google Drive:

**Dataset Numérico + Textos + Imagens**

Link:
https://drive.google.com/drive/folders/1PaNLIwWO2_WT7sCM-djmNTPAsQjAru-5?usp=drive_link


---

# Considerações sobre Governança de Dados

Durante a coleta e organização dos dados foram considerados alguns princípios de Governança de Dados:

- organização estruturada dos datasets
- separação por tipo de dados (numérico, textual e visual)
- documentação clara da origem das informações
- preparação para uso em modelos de Inteligência Artificial

Também é importante considerar que dados médicos podem conter **viés**, como diferenças demográficas ou amostras limitadas. Em projetos reais, seria necessário ampliar a diversidade dos dados e garantir representatividade adequada.

---

# Conclusão

A construção desta base de dados representa o primeiro passo para o desenvolvimento do sistema **CardioIA**. 

Com dados numéricos, textuais e visuais organizados, será possível nas próximas fases aplicar algoritmos de **Machine Learning, NLP e Visão Computacional** para gerar análises inteligentes e apoiar decisões na área da saúde cardiovascular.
