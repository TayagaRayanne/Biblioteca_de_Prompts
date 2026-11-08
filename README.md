# 📚 Biblioteca Pessoal de Prompts & Governança de Contexto (Prompt Vault)

## 📌 Origem, Visão e Propósito Permanente
Esta biblioteca foi concebida a partir do **Projeto de Encerramento do Módulo de Engenharia de Prompt**, componente formativo do programa **ADA - Nuclea Ser+ Tech - Formação em IA**. 

Embora o estalo inicial tenha surgido no ambiente acadêmico como resposta aos desafios de mitigação de riscos, limitações de LLMs e conformidade com a LGPD, esta biblioteca transcende o escopo do curso: **ela foi instituída como um ativo de engenharia de software e repositório pessoal permanente**. O objetivo é centralizar, versionar e armazenar de forma segura os melhores prompts desenvolvidos para diferentes áreas de atuação profissional, evitando o uso empírico e descartável de ferramentas de IA no dia a dia.

---

## 🏛️ Diretrizes Arquiteturais (Padrão de Engenharia)
Todos os artefatos armazenados nesta biblioteca respeitam os padrões de qualidade e segurança validados no módulo:

1. **Framework C.P.T.F. como Padrão de Projeto:**
   - **[C] Contexto:** Ancoragem de domínio, regras de negócio e limites de contexto.
   - **[P] Persona:** Definição técnica de papel com viés pragmático e sem otimismo artificial.
   - **[T] Tarefa:** Decomposição algorítmica e passos sequenciais de execução.
   - **[F] Formato:** Contrato estrito de interface e saída (Markdown, JSON Schema, tabelas).

2. **Segregação de Responsabilidades (Determinismo vs. Probabilidade):**
   - Modelos de linguagem atuam na camada semântica (classificação, síntese, inferência e raciocínio textual).
   - Agregações financeiras, cálculos métricos e contagens numéricas permanecem delegados a planilhas, consultas SQL ou scripts Python determinísticos.

3. **Governança e Blindagem Ativa de Segurança:**
   - **Regra Zero (Anti-Injection):** Textos externos e dados não confiáveis são tratados como dados passivos, anulando ordens embutidas.
   - **Privacidade por Design (LGPD):** Anonimização prévia em duas camadas e substituição mandatória de PII pela máscara `[DADO PESSOAL OCULTO]`.
   - **Diretriz Anti-Leak:** Preservação estrita das instruções internas de sistema contra engenharia social ou falsa autoridade.
   - **Compromisso Ético e Veracidade:** Rejeição explícita a alucinações, adulteração de fatos ou falsificação curricular.

---

## 📂 Mapa de Diretórios
* `/templates`: Templates reutilizáveis com variáveis dinâmicas (`{{VARIAVEL}}`) para acelerar a criação de novos prompts.
* `/prompts/analise_dados`: Prompts para triagem operacional, classificação semântica e sumarização executiva de bases de dados (ex.: Caso Tucano Pay).
* `/prompts/carreira_recrutamento`: Prompts para auditoria de requisitos de vagas, Gap Analysis e estratégias de posicionamento de currículo (ex.: Tay Career Scout).
* `/prompts/engenharia_software`: Prompts focados em arquitetura back-end (Python/FastAPI), revisão de código, modelagem relacional (SQL) e suítes de testes unitários (pytest).
* `/prompts/automacao_rpa`: Prompts voltados para estruturação de fluxos no n8n, webhooks e conteinerização com Docker.
* `/seguranca`: Checklists operacionais e protocolos de teste de estresse (Red Teaming).

---

## 🔄 Fluxo de Versionamento e Manutenção
- **Versionamento Semântico:** Cada prompt possui identificador único (`PRM_DOM_000`) e controle de versão (`v1.0`, `v1.1`).
- **Homologação:** Nenhum prompt é catalogado como estável sem antes passar pela validação nominal e pelo checklist de Red Teaming contra injeções adversariais.
