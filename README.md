```mermaid
flowchart TD
  A(["Inicio"])
  A --> B{"Faça uma escolha"}
  B --> C["OP1"]
  B --> E["OP2"]
  B --> D["OP3"]
```

```mermaid
graph TD;
A[Inicio] --> B{Nota > 6};
B --> |SIM| C[Aprovado];
B --> |NÃO| D[Reprovado];
```

```mermaid
gantt
  title Exemplo de Gráfico de Gantt
  dateFormat YYYY-MM-DD
  section 1ºSemestre
  1º Bimestre ✅ Finalizado:done, a1, 2025-02-02, 60d
  2º Bimestre ✅ Finalizado:done, a2, after a1, 60d
  section 2ºSemestre
  3º Bimestre ⏳Em Andamento:active, a3, 2025-08-01, 60d
  4º Bimestre ⏳Em Andamento:crit, a4, after a3, 60d
```
Exercício não avaliativo

```mermaid
gantt
    title Construção de uma Casa
    dateFormat DD-MM-YYYY
    axisFormat %d/%m

    section Fase 1: Fundação
    Fundação :a1, 10-09-2025, 15d

    section Fase 2: Estrutura
    Estrutura da Casa :a2, after a1, 30d

    section Fase 3: Instalações
    Instalações Elétricas e Hidráulicas :a3, after a2, 20d

    section Fase 4: Acabamento
    Acabamento Interno :a4, after a3, 25d
    Acabamento Externo :a5, after a4, 15d

    section Fase 5: Finalização
    Inspeção e Entrega :a6, after a5, 5d
```
```mermaid
gantt
    title Projeto: Sistema de Cadastro de Empresas
    dateFormat  YYYY-MM-DD
    -- Define o formato do eixo para mostrar o número da semana
    axisFormat %W
    
    %% O projeto tem duração de 24 semanas. Início em 06/10/2025.

    section Fase 1: Planejamento e Análise
    Levantamento de Requisitos    :crit, done, 2025-10-06, 1w
    Documentação Funcional        :done, 2025-10-06, 10d

    section Fase 2: Design de Interface (UI/UX)
    Elaboração de Wireframes      :done, after Levantamento de Requisitos, 1w
    Criação do Layout Definitivo  :done, after Elaboração de Wireframes, 2w

    section Fase 3: Configuração e Desenvolvimento
    Config. Ambiente e Git        :crit, done, 2025-10-06, 1w
    Criação do Banco de Dados     :done, after Config. Ambiente e Git, 1w
    Entrega 1: Módulo de Login   :active, 2025-10-20, 2w
    Entrega 2: CRUD de Empresas   :2025-11-03, 3w
    Entrega 3: Upload de Logotipo :2025-11-24, 2w
    Entrega 4: Relatórios         :2025-12-08, 2w
    Entrega 5: Painel Admin       :2025-12-22, 2w

    section Fase 4: Testes e Validação
    Testes Unitários e Integração :crit, 2025-10-20, 18w
    Testes de Usabilidade         :after Entrega 5, 2w
    Correção de Bugs              :after Testes de Usabilidade, 6w

    section Fase 5: Implantação e Encerramento
    Prep. Ambiente de Produção    :2026-03-02, 1w
    Implantação Final (Go-live)   :after Prep. Ambiente de Produção, 1w
    Validação e Treinamento       :after Implantação Final (Go-live), 1w
    Encerramento do Projeto       :after Validação e Treinamento, 1w
```
