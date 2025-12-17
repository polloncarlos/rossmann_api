<h1>📦 Rossmann Sales Forecast API</h1>

<p>
API em <b>Flask</b> para previsão de vendas das lojas Rossmann utilizando um modelo
<b>XGBoost</b>, desenvolvida como camada de produção de um projeto completo de
<b>Ciência de Dados</b>.
</p>

<hr/>

<h2>📌 Visão Geral</h2>

<p>
Este projeto disponibiliza uma <b>API REST</b> capaz de prever as vendas das lojas
Rossmann para um horizonte de <b>6 semanas</b>, utilizando dados históricos e
informações contextuais das lojas.
</p>

<p>
A API representa a etapa final de um pipeline de Data Science, iniciado com
análise exploratória, modelagem e validação, e finalizado com a entrega de um
produto consumível em produção.
</p>

<ul>
  <li>Arquitetura limpa e desacoplada</li>
  <li>Serialização de modelo e preprocessadores</li>
  <li>Inferência em tempo real</li>
  <li>Integração com serviços externos</li>
</ul>

<hr/>

<h2>🏗️ Arquitetura</h2>

<pre>
Cliente (Bot / App / Serviço)
        |
        v
   Flask REST API
        |
        v
   Pipeline de Pré-processamento
        |
        v
   Modelo XGBoost
        |
        v
 Previsão de Vendas (JSON)
</pre>

<hr/>

<h2>⚙️ Stack Tecnológica</h2>

<ul>
  <li>Python</li>
  <li>Flask</li>
  <li>Pandas / NumPy</li>
  <li>Scikit-learn</li>
  <li>XGBoost</li>
  <li>Gunicorn</li>
  <li>Deploy em Render</li>
</ul>

<hr/>

<h2>🔮 Modelo</h2>

<ul>
  <li><b>Algoritmo:</b> XGBoost Regressor</li>
  <li><b>Horizonte de previsão:</b> 6 semanas</li>
  <li><b>Entrada:</b> Dados históricos e features das lojas</li>
  <li><b>Saída:</b> Previsão de vendas por loja</li>
</ul>

<p>
O modelo foi validado utilizando técnicas de cross-validation e otimização de
hiperparâmetros, sendo carregado em produção exclusivamente para inferência.
</p>

<hr/>

<h2>🌐 Deploy</h2>

<p>
A API está publicada como um <b>Web Service</b> no Render, utilizando Gunicorn,
simulando um ambiente real de produção com recursos limitados.
</p>

<ul>
  <li>Serviço stateless</li>
  <li>Pronto para consumo externo</li>
  <li>Integração via HTTP</li>
  <li>Compatível com plano gratuito</li>
</ul>

<hr/>

<h2>🔗 Integrações</h2>

<p>
🤖 <b>Telegram Bot</b><br/>
A API é consumida pelo projeto
<a href="https://github.com/polloncarlos/rossmann_telegram_bot">
rossmann_telegram_bot
</a>, permitindo que usuários obtenham previsões diretamente via Telegram.
</p>

<hr/>

<h2>📈 Próximas Evoluções</h2>

<ul>
  <li>Camada de autenticação</li>
  <li>Validação de payload</li>
  <li>Suporte a previsões em lote</li>
  <li>Monitoramento e logging</li>
</ul>
