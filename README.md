# 🏎️ Porsche Sales Analytics Dashboard

Dashboard interativa de desempenho de vendas da Porsche desenvolvida para o desafio de projeto DIO. O projeto transforma uma base de dados sanitizada de 100 transações comerciais em um painel responsivo em HTML/JS, sem limitações do Excel e com publicação gratuita no GitHub Pages.

🔗 **Dashboard Online:** https://laurabgularte.github.io/dashboard-porsche-dio/

---

## 📌 1. Perguntas de Negócio Respondidas

1. **Quais modelos e famílias da Porsche geram a maior receita total?**
   * *Justificativa:* Permite separar modelos de alto volume financeiro (como a linha 911 e Taycan Turbo) dos modelos de entrada, alinhando a estratégia comercial e de importação.
2. **Qual a participação de cada Método de Pagamento na receita global?**
   * *Justificativa:* Identifica a adesão dos clientes a modalidades como *Wire Transfer*, *Financing* e *Crypto Payment*, otimizando negociações de taxas financeiras.
3. **Quais Estados e regiões concentram os maiores volumes de vendas?**
   * *Justificativa:* Mapeia a presença territorial da marca para subsidiar decisões de marketing regional e abertura de novas concessionárias.

---

## 🛠️ 2. Tratamento da Base de Dados

* **Filtro de Colunas Sanitizadas:** Extração direta dos dados higienizados nas Aulas DIO (`PorscheModelSanitized`, `SalesPriceSanitized`, etc.).
* **Padronização Tipológica:** Limpeza de símbolos monetários e conversão de preços e anos para valores estritamente numéricos.
* **Mapeamento de Famílias:** Agrupamento por categorias (`911`, `Cayenne`, `Taycan`, `Panamera`, `Macan`, `718`) para filtragem rápida.

---

## 🤖 3. Prompt Utilizado na Geração pelo Canvas / ChatGPT

```text
Crie uma dashboard interativa de vendas da Porsche em arquivo único HTML/JS com as seguintes especificações:
1. Tema e Estilo: Dark mode elegante (Porsche Red #E30613, Dourado #D4AF37, fundo #0B0E14), componentes com Tailwind CSS e gráficos Chart.js.
2. KPIs no Topo: Receita Total, Volume de Transações, Ticket Médio e Modelo Mais Vendido.
3. Três Gráficos de Negócio:
   - Gráfico de barras horizontais: Receita por Modelo.
   - Gráfico de rosca: Distribuição por Método de Pagamento.
   - Gráfico de barras verticais: Top Estados em Faturamento.
4. Filtros Interativos: Família de veículos, Estado, Método de Pagamento e Status. A alteração de qualquer filtro deve recalcular dinamicamente todos os KPIs e gráficos.
5. Tabela Detalhada com busca e dados sanitizados embutidos em JS.
