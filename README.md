# Guia de Estudos: Assessor de Criptoativos e Suporte em Blockchain com NotebookLM

## Contexto e Objetivos

Este repositório apresenta o projeto prático desenvolvido para o desafio de projeto da DIO. O objetivo é utilizar o **Google NotebookLM** como uma ferramenta de aprendizagem ativa inteligente para estruturar um **Assessor de Investimentos Cripto, Regulação e Infraestrutura Blockchain**.

A ferramenta foi alimentada com bases de dados dinâmicas (textos e vídeos) para atuar em três pilares estratégicos:
1.  **Suporte de Engenharia e Arquitetura**: Esclarecer mecânicas profundas de protocolos de primeira camada (L1), segunda camada (L2) e contratos inteligentes.
2.  **Compliance e Regulação**: Fornecer respostas ágeis sobre os impactos regulatórios globais e nacionais no ecossistema cripto.
3.  **Análise de Mercado**: Mitigar riscos de assimetria de informação através da leitura analítica de novidades e fluxos de liquidez.

*   **Link do Notebook Gerado**: https://notebooklm.google.com/notebook/76d60cbd-13d2-4c21-bf71-8746bced4a18

---

## Curadoria de Fontes

O modelo foi contextualizado a partir de uma curadoria mista (multimodal), integrando análises de portais de referência global e conteúdos audiovisuais de alta densidade técnica.

### 🎥 Fontes de Vídeo (Análises, Tutoriais e Cenários)
*   [Vídeo Base 1 - Cenários e Fundamentos](https://www.youtube.com/watch?v=McrsVDAW6xg)
*   [Vídeo Base 2 - Infraestrutura Blockchain](https://www.youtube.com/watch?v=hKuqlbbadWM)
*   [Vídeo Base 3 - Regulação e Ativos](https://www.youtube.com/watch?v=lkhn-spn-IA)
*   [Vídeo Base 4 - Macroeconomia e Cripto](https://www.youtube.com/watch?v=6o95K_eqS04)
*   [Vídeo Base 5 - Fluxos de Liquidez](http://youtube.com/watch?v=dm13kLK0hT0)
*   [Vídeo Base 6 - Smart Contracts Avançados](https://www.youtube.com/watch?v=amiIOs-lMS0)
*   [Vídeo Base 7 - Protocolos DeFi e Riscos](https://www.youtube.com/watch?v=h47hCNdt-xQ)
*   [Vídeo Base 8 - Tendências Globais de Mercado](https://www.youtube.com/watch?v=BslEUBLr51g)

### Fontes de Texto (Notícias, Dados de Mercado e Regulação)
*   [CoinDesk Portugal](https://www.coindesk.com/pt-br) - Referência em jornalismo de ativos digitais e atualizações regulatórias.
*   [BlockTrends](https://blocktrends.com.br/) - Análise de dados On-Chain, macroeconomia e mercado institucional.
*   [Observatório Blockchain](https://observatorioblockchain.org.br/) - Pesquisas acadêmicas, governança jurídica e ecossistema local.
*   [Yahoo Finance Crypto](https://finance.yahoo.com/markets/crypto/all/) - Dados financeiros agregados em tempo real, tickers e métricas de preço.

---

## Engenharia de Prompts e Troubleshooting

Para avaliar a maturidade do Assessor e mitigar riscos de alucinação, foram aplicados três níveis de testes: Prompts de Escopo, Filtros de Fronteira e Testes de Precisão Numérica.

### 1. Prompts de Negócio e Infraestrutura (Alineados ao Tema)
*   **Prompt 1:** *Como as stablecoins estão revolucionando as remessas internacionais de dinheiro?*
*   **Prompt 2:** *Quais as dificuldades e desafios de se implantar stablecoins (riscos de descolamento de paridade, liquidez e barreiras fiduciárias)?*
*   **Prompt 3:** *Existem carteiras restritas e proibidas de se transacionar na blockchain (Mapeamento de sanções da OFAC e Blacklisting)?*
*   **Resultado:** O NotebookLM forneceu respostas altamente coerentes. Ele diferenciou com precisão o congelamento a nível de protocolo (centralizado em emissores como Tether/Circle) da imutabilidade nativa de redes descentralizadas.

### 2. Teste de Integridade: Filtro de Fronteira de Conhecimento
*   **Prompt:** *Quanto custa um iphone 17?*
*   **Análise do Erro/Comportamento:** O objetivo do teste era verificar se a IA extrapolaria a base fornecida ou alucinaria com dados externos não homologados. A IA demonstrou forte alinhamento com as fontes do repositório, pontuando que o assunto fugia ao escopo e citando um valor meramente hipotético extraído de um contexto comparativo de preços presente em uma das matérias indexadas.

### 3. Teste de Estresse de Alucinação: Precisão Matemática (Sub-Satoshi)
*   **Prompt:** *Quanto eu gastaria em reais para comprar 0,000000005 BTC?*
*   **Análise do Acerto:** O prompt continha uma "pegadinha" matemática: a quantia inserida representa exatamente **0,5 Satoshi** (metade da menor unidade fracionária possível de ser registrada na camada principal da Blockchain do Bitcoin, onde 1 Satoshi = 10⁻⁸ BTC ou `0,00000001 BTC`). O NotebookLM captou com sucesso a inserção intencional do dígito zero excedente, validando a sua integridade para cálculos e análises financeiras granulares.

---

## Miniguia de Estudo

### Resumos Estruturados do Assunto

*   **A Evolução das Remessas Globais**: O uso de Stablecoins pareadas ao Dólar americano (como USDT e USDC) tende a transformar remessas internacionais. O processo reduz o tempo de liquidação financeira de dias úteis (padrão SWIFT) para minutos, eliminando intermediários bancários e reduzindo as taxas de conversão cambial (*spread*).
*   **O Desafio da Regulamentação Global**: O mercado cripto enfrenta uma transição rápida rumo à institucionalização. Protocolos DeFi e emissores de stablecoins operam sob crescente cautela de frameworks globais (como o regulamento MiCA na Europa e diretrizes do Banco Central/CVM no Brasil), forçando a adoção de regras rígidas de conformidade.
*   **Rastreabilidade vs. Anonimato**: Embora a infraestrutura blockchain seja descentralizada, ela é pública. Agências reguladoras utilizam ferramentas de análise *On-Chain* para monitorar movimentações fraudulentas e aplicar restrições a endereços vinculados a atividades ilícitas (*Blacklisting*).

### Glossário de Conceitos Chave

*   **Satoshi:** A menor unidade de medida fracionária do Bitcoin. Equivale a 10⁻⁸ BTC, ou seja, `0,00000001 BTC`.
*   **Stablecoin:** Criptoativo emitido com o objetivo de manter paridade de preço estável com um ativo de referência, geralmente moedas tradicionais como o Dólar (USDT/USDC) ou commodities como o Ouro.
*   **Blacklisting (Lista Negra):** Mecanismo presente no código de alguns contratos inteligentes de stablecoins centralizadas que permite ao emissor congelar fundos e impedir que um endereço específico transacione na rede.
*   **Análise On-Chain:** O processo de examinar os dados brutos históricos e em tempo real registrados diretamente no livro-razão público da blockchain (como volume de transações, taxas e balanço de carteiras).
*   **Descolamento de Paridade (De-peg):** Fenômeno financeiro onde uma estável perde a sua equivalência/paridade de 1:1 com o ativo lastreado (EURO ou DOLAR por exemplo).

### Prompts Reutilizáveis para Revisão e Auditoria

```text
Prompt 1: "Com base nas análises de mercado extraídas da CoinDesk e BlockTrends contidas nesta pasta, quais são as principais atualizações regulatórias sobre a conformidade de stablecoins que podem impactar investidores da América Latina neste trimestre?"
```

```text
Prompt 2: "Atue como um especialista em segurança blockchain. Sintetize os principais riscos operacionais associados ao fornecimento de liquidez em protocolos DeFi, considerando as fontes de vídeo anexadas."
```
