# Ferramentas grátis e open source, por área

> **Legenda de licenças**
> - **MIT / Apache-2.0 / BSD / ISC / Unlicense**: livre pra tudo, inclusive modificar, fechar o código e revender.
> - **AGPL / GPL / LGPL / MPL**: livre e grátis. Se você modificar e oferecer pela rede (AGPL) ou distribuir (GPL), precisa abrir o código modificado. Usar sem modificar, como serviço separado, é tranquilo.
> - **Freemium**: serviço online com plano grátis que ainda tem utilidade real. O limite grátis vai indicado.
> - **⚠️**: licença com restrição (não é open source de verdade, ou proíbe revender/oferecer como serviço) ou licença própria que precisa ser conferida. Leia antes de usar com cliente.
> - **"+ Enterprise pago"**: o núcleo é livre, mas há uma pasta (`ee/`, `enterprise/`) com recursos pagos no mesmo repositório. Não ative esses recursos sem licença.

## Índice

**Negócio e operação**
1. [Prospecção B2B](#1-prospecção-b2b)
2. [CRM, atendimento e comunicação](#2-crm-atendimento-e-comunicação)
3. [Automação e low-code](#3-automação-e-low-code)
4. [E-mail, outreach e newsletter](#4-e-mail-outreach-e-newsletter)
5. [Redes sociais](#5-redes-sociais)
6. [Analytics, conversão e SEO](#6-analytics-conversão-e-seo)
7. [Formulários e captação de leads](#7-formulários-e-captação-de-leads)
8. [Finanças, faturamento e ERP](#8-finanças-faturamento-e-erp)
9. [Documentos e assinatura](#9-documentos-e-assinatura)
10. [Produtividade e conhecimento](#10-produtividade-e-conhecimento)
11. [E-commerce](#11-e-commerce)
12. [Autenticação e identidade](#12-autenticação-e-identidade)

**Dev e infraestrutura**

13. [Sites, CMS, backend e armazenamento](#13-sites-cms-backend-e-armazenamento)
14. [Infraestrutura, deploy e hospedagem](#14-infraestrutura-deploy-e-hospedagem)
15. [Testes e segurança](#15-testes-e-segurança)
16. [Monitoramento e observabilidade](#16-monitoramento-e-observabilidade)
17. [Produtividade de dev](#17-produtividade-de-dev)
18. [IA](#18-ia)
19. [Utilitários e outros](#19-utilitários-e-outros)

**Design e front-end**

20. [Design](#20-design)
21. [Front-end: componentes e interface](#21-front-end-componentes-e-interface)
22. [Ajuste visual com IA (localhost)](#22-ajuste-visual-com-ia-localhost)
23. [Skills e recursos anti-"cara de IA"](#23-skills-e-recursos-anti-cara-de-ia)
24. [Qualidade de UI: linters, acessibilidade e performance](#24-qualidade-de-ui-linters-acessibilidade-e-performance)
25. [Referências de estudo e inspiração](#25-referências-de-estudo-e-inspiração)

---

# NEGÓCIO E OPERAÇÃO

## 1. Prospecção B2B

### 1.1 Dados de empresas: Brasil

| Ferramenta | Licença | O que faz |
|---|---|---|
| [minhareceita.org](https://docs.minhareceita.org) | Open source | Consulta tudo de um CNPJ: atividade (CNAE), porte, sócios, endereço e data de abertura. Dá pra usar a API pública ou rodar a base inteira no seu servidor e filtrar como quiser. |
| [BrasilAPI](https://brasilapi.com.br) | Open source | API grátis e sem cadastro pra consultar CNPJ, CEP e afins. Boa pra scripts rápidos, mas sem garantia de que vai estar no ar. |
| [Casa dos Dados](https://casadosdados.com.br) | Freemium (consulta individual + 20 resultados por busca avançada) | Busca empresas por atividade, cidade e data de abertura. Serve pra testar filtros antes de montar sua própria base. |
| [Dados abertos CNPJ](https://dados.gov.br) | Dados públicos | Arquivos brutos mensais com todas as empresas do Brasil. Pra quem quer importar tudo num banco próprio. |
| [CNA / CNSA – OAB](https://cnsa.oab.org.br) | Cadastro oficial grátis | Consulta advogados e sociedades de advocacia, com sócios, endereço e telefone do escritório. |
| OAB-SP – Consulta de Sociedades | Cadastro oficial grátis | Lista escritórios de SP, com filtro específico para "Sociedades de Consultores em Direito Estrangeiro". |

### 1.2 Dados de empresas: Portugal

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Publicações de Atos Societários](https://publicacoes.mj.pt) | Oficial, grátis | Mostra sócios, gerência, capital e empresas recém-constituídas. Busca por NIPC, data e concelho, sem cadastro. |
| [empresadb.pt](https://empresadb.pt) | Grátis | Lista empresas por setor (CAE), concelho e freguesia, sem precisar de conta. |
| [Racius](https://racius.com) | Freemium (navegação e relatório básico grátis) | Navega empresas por CAE e distrito, e avisa por e-mail quando uma empresa que você segue muda algo. |
| [eInforma](https://einforma.pt) | Freemium (5 relatórios grátis + monitorização) | Relatórios de empresas (vendas, gestores, risco) e alerta de mudanças nas empresas que você acompanha. |
| [SICAE](https://sicae.pt) | Oficial, grátis | Confirma a atividade principal e secundária (CAE) de uma empresa. |
| [Ordem dos Advogados](https://portal.oa.pt) | Oficial, grátis | Pesquisa advogados e sociedades de advogados por localidade. |

### 1.3 Scraping (extrair dados de sites)

| Ferramenta | Licença | O que faz |
|---|---|---|
| [google-maps-scraper (gosom)](https://github.com/gosom/google-maps-scraper) | MIT | Extrai empresas do Google Maps: nome, telefone, site, avaliações e até o e-mail do site. Roda no seu servidor, sem limite. Viola os termos do Google, então use em volume baixo. |
| [Crawl4AI](https://github.com/unclecode/crawl4ai) | Apache-2.0 | Raspa sites e devolve o texto limpo (Markdown/JSON), pronto pra uma IA extrair nome de sócio, e-mail, áreas de atuação. |
| [Firecrawl](https://firecrawl.dev) | AGPL (self-host) / Freemium (1.000 páginas/mês) | API que transforma páginas da web em dados estruturados. |
| [Scrapy](https://scrapy.org) | BSD | Framework Python pra robôs de raspagem grandes, com várias páginas. |
| [Apify](https://apify.com) | Freemium (US$ 5/mês em créditos) | Plataforma com robôs de raspagem prontos (Maps, diretórios etc.), sem precisar de servidor. |
| [Instant Data Scraper](https://chromewebstore.google.com) | Grátis (extensão Chrome) | Copia tabelas e listas de qualquer site pra CSV com um clique. |

### 1.4 Encontrar e validar e-mails de decisores

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Reacher (check-if-email-exists)](https://github.com/reacherhq/check-if-email-exists) | AGPL-3.0 (ou comercial) | Verifica se um e-mail existe sem mandar mensagem. Self-host, sem limite, mas precisa da porta 25 aberta no servidor. |
| [Hunter.io](https://hunter.io) | Freemium (50 créditos/mês; campanhas: 1 caixa, 500 destinatários) | Descobre o padrão de e-mail de um domínio (ex.: nome.sobrenome@), verifica e-mails e envia sequências simples a partir do seu Gmail. Ótimo pra escritórios com site próprio. |
| [Apollo.io](https://apollo.io) | Freemium (~75 créditos/mês) | Base gigante de contatos B2B, com busca por cargo. Fraca em pequenas empresas BR/PT. |
| [Snov.io](https://snov.io) | Freemium (50 créditos + 100 destinatários) | Busca e verifica e-mails e envia campanhas pequenas. Tem extensão de LinkedIn. |
| [GetProspect](https://getprospect.com) | Freemium (50 e-mails + 100 verificações) | Extensão simples pra achar e-mails a partir do LinkedIn. |
| [Kaspr](https://kaspr.io) | Freemium (15 e-mails + 5 telefones) | Contatos com foco na Europa. ⚠️ Foi multada pela CNIL (França) por coletar dados do LinkedIn. |
| [Lusha](https://lusha.com) | Freemium (~40 créditos) | Mais forte em telefone direto. Cobertura BR/PT irregular. |

### 1.5 Sinais de oportunidade (quem abordar e quando)

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Google Trends](https://trends.google.com) / [Google Alerts](https://google.com/alerts) | Grátis | Acompanha buscas e notícias do nicho (ex.: "AIMA", "visto D7") pra acertar o timing da abordagem. |
| [changedetection.io](https://github.com/dgtlmoon/changedetection.io) | Apache-2.0 | Vigia páginas e avisa quando algo muda (preço, texto, vaga, edital). Também serve pra acompanhar o site de concorrentes e de leads. |
| LinkedIn Jobs, Net-Empregos, Indeed, Gupy | Grátis | Vagas abertas revelam dor operacional (ex.: contratando "assistente de processos de imigração"). |
| [PNCP](https://pncp.gov.br) (BR), [BASE.gov](https://base.gov.pt) (PT), [TED](https://ted.europa.eu) (UE) | Grátis | Editais e compras públicas, ex.: digitalização de pequenas empresas e municípios. |
| Barómetro / Firmografia Informa D&B | Grátis | Números de mercado em Portugal por concelho e setor. |

---

## 2. CRM, atendimento e comunicação

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Twenty](https://github.com/twentyhq/twenty) | AGPL-3.0 + Enterprise pago | CRM moderno pra rodar no seu servidor, sem limite de usuários nem de registros. Campos e visões personalizáveis, API GraphQL. |
| [EspoCRM](https://espocrm.com) | AGPL | CRM leve e completo pra self-host. |
| [SuiteCRM](https://suitecrm.com) | AGPL | CRM tradicional, robusto, mais pesado. |
| [Odoo Community](https://odoo.com) | LGPL | CRM + ERP (financeiro, estoque etc.) no mesmo sistema. |
| [Krayin](https://krayincrm.com) | MIT | CRM em Laravel, simples. |
| [Attio](https://attio.com) | Freemium (3 usuários, 50.000 registros) | CRM online com o plano grátis mais generoso em volume. |
| [HubSpot Free](https://hubspot.com) | Freemium (2 usuários, 1.000 contatos) | CRM online sem manutenção, com rastreio de e-mail. |
| [Zoho CRM Free](https://zoho.com/crm) | Freemium (3 usuários, 5.000 registros) | CRM online, mais espaço que o Bigin, interface mais pesada. |
| [Zoho Bigin](https://bigin.com) | Freemium (1 usuário, 500 registros) | Funil de vendas simples pra um negócio só. |
| [Chatwoot](https://github.com/chatwoot/chatwoot) | MIT + Enterprise pago | Central de atendimento: junta chat do site, WhatsApp, e-mail e redes numa caixa só. Pode revender. |
| [Fluxer](https://github.com/fluxerapp/fluxer) | AGPL-3.0 | Chat e chamadas de voz/vídeo estilo Discord/Slack, no seu servidor. Serve pra equipe ou comunidade de cliente. |
| [Cal.diy](https://github.com/calcom/cal.diy) | MIT | Agendamento online (versão aberta do Cal.com). Sem equipes, round-robin nem workflows; oficialmente recomendado só pra uso pessoal. |
| [WhatsApp Business (app)](https://business.whatsapp.com) | Grátis | Catálogo, etiquetas de funil e respostas rápidas no WhatsApp. |
| [Evolution API](https://github.com/EvolutionAPI/evolution-api) | ⚠️ Apache-2.0 com condições | API de WhatsApp muito usada no Brasil. Obriga manter a marca e um aviso de uso. Envio em massa pela versão não oficial pode banir o número. |

---

## 3. Automação e low-code

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Activepieces](https://github.com/activepieces/activepieces) | MIT + Enterprise pago | Automações tipo Zapier ("quando chega X, faz Y"), com 400+ conectores e agentes de IA. Pode embutir e revender. |
| [Windmill](https://github.com/windmill-labs/windmill) | AGPL-3.0 (opção comercial) | Transforma scripts (Python, TypeScript, Go, Bash, SQL) em APIs, tarefas agendadas, workflows e telas. Alternativa ao Retool/Pipedream pra ferramentas internas. |
| [ToolJet](https://github.com/ToolJet/ToolJet) | AGPL-3.0 | Monta painéis e sistemas internos arrastando componentes, ligando em bancos e APIs. Alternativa ao Retool/Appsmith. |
| [n8n](https://n8n.io) | ⚠️ Sustainable Use License | Automação poderosa, grátis pra uso interno, mas proíbe oferecer como serviço a terceiros. Pra revender, use Activepieces. |

---

## 4. E-mail, outreach e newsletter

| Ferramenta | Licença | O que faz |
|---|---|---|
| [listmonk](https://github.com/knadh/listmonk) | AGPL-3.0 | Newsletter e listas de e-mail, leve, num servidor só. Pra base que pediu pra receber (não pra e-mail frio). |
| [Mautic](https://github.com/mautic/mautic) | GPL-3.0 | Automação de marketing (jornadas, pontuação de leads). Substitui RD Station/HubSpot Marketing. Pesado. |
| [useSend](https://github.com/usesend/useSend) | AGPL-3.0 | Envio de e-mails transacionais (confirmações, senhas) sobre o Amazon SES. Alternativa ao Resend/SendGrid. |
| [Postal](https://github.com/postalserver/postal) | MIT | Servidor de envio de e-mail completo. Só se você souber cuidar de reputação de IP. |
| [React Email](https://github.com/resend/react-email) | MIT | Escreve templates de e-mail em React. |
| [MJML](https://github.com/mjmlio/mjml) | MIT | Linguagem que gera e-mail responsivo que funciona até no Outlook. |

*(Para campanhas de e-mail frio simples, ver Hunter e Snov.io na seção 1.4.)*

---

## 5. Redes sociais

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Postiz](https://github.com/gitroomhq/postiz-app) | AGPL-3.0 | Agenda posts em 20+ redes, com IA e API. Self-host sem recursos bloqueados. Alternativa ao Buffer/Hootsuite. |
| [Mixpost Lite](https://github.com/inovector/mixpost) | MIT | Agendador de posts em Laravel (PHP). |
| [LinkStack](https://github.com/LinkStackOrg/LinkStack) | AGPL-3.0 | "Link na bio" tipo Linktree, com domínio próprio. |
| [LittleLink](https://github.com/sethcottle/littlelink) | MIT | "Link na bio" estático, sem backend. |

---

## 6. Analytics, conversão e SEO

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Umami](https://github.com/umami-software/umami) | MIT | Analytics de site sem cookies (não precisa de banner LGPD/RGPD). Leve e pode ter sua marca. |
| [Plausible CE](https://github.com/plausible/analytics) | AGPL-3.0 | Analytics sem cookies, com painel mais polido. |
| [OpenPanel](https://github.com/Openpanel-dev/openpanel) | AGPL-3.0 | Analytics de produto: eventos, funis, retenção (tipo Mixpanel). |
| [PostHog](https://github.com/PostHog/posthog) | MIT + Enterprise pago | Analytics, gravação de sessão, feature flags e testes A/B. Pesado pra servidor pequeno. |
| [GrowthBook](https://github.com/growthbook/growthbook) | MIT | Testes A/B e feature flags. |
| [Dub](https://github.com/dubinc/dub) | AGPL-3.0 + Enterprise pago | Encurtador de links com rastreio de cliques e UTMs, no domínio do cliente. |
| [SerpBear](https://github.com/towfiqi/serpbear) | MIT | Acompanha a posição das palavras-chave no Google. |
| [Unlighthouse](https://github.com/harlan-zw/unlighthouse) | MIT | Roda o Lighthouse em todas as páginas do site de uma vez. Auditoria de SEO técnico. |
| [Web-Check](https://github.com/Lissy93/web-check) | MIT | Analisa qualquer site de uma vez: certificado SSL, DNS, portas abertas, tecnologias usadas, SEO, performance. Ótimo pra auditoria e análise de concorrente. |

---

## 7. Formulários e captação de leads

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Formbricks](https://github.com/formbricks/formbricks) | AGPL-3.0 + Enterprise pago | Formulários, pesquisas, NPS e pop-ups. Captura lead e coleta depoimento no mesmo lugar. |
| [OpnForm](https://github.com/OpnForm/OpnForm) | AGPL-3.0 | Criador de formulários estilo Typeform/Tally, com webhooks. |
| [LimeSurvey](https://github.com/LimeSurvey/LimeSurvey) | GPL-2.0 | Pesquisas longas com lógica complexa. |
| [Typebot](https://github.com/baptisteArno/typebot.io) | ⚠️ FSL-1.1 | Chatbot/formulário conversacional. Pode usar internamente, mas não pode revender a hospedagem. |

---

## 8. Finanças, faturamento e ERP

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Invoicerr](https://github.com/invoicerr-app/invoicerr) | AGPL-3.0 | Orçamentos e faturas para freelancer: gera PDF, envia por e-mail, coleta assinatura e controla pagamentos. |
| [Crater](https://github.com/crater-invoice-inc/crater) | AGPL-3.0 | Faturas e orçamentos com despesas, faturas recorrentes e app de celular. Alternativa ao FreshBooks. |
| [TaxHacker](https://github.com/vas3k/TaxHacker) | MIT | Você joga recibos e notas em PDF/foto e a IA lê, categoriza e organiza despesas. Exporta pra Excel/CSV pro contador. |
| [Kimai](https://github.com/kimai/kimai) | AGPL-3.0 | Controle de horas por cliente e projeto, com relatórios e faturas. Bom pra cobrar por hora. |
| [IDURAR](https://github.com/idurar/idurar-erp-crm) | AGPL-3.0 | ERP/CRM simples: clientes, orçamentos, faturas, estoque e contabilidade básica. |
| [ERPNext](https://github.com/frappe/erpnext) | GPL-3.0 | ERP completo: contabilidade, estoque, CRM, projetos, RH e folha. Substitui várias ferramentas, mas é grande. |
| [OpenBB](https://github.com/OpenBB-finance/OpenBB) | ⚠️ Licença própria (conferir) | Plataforma de dados financeiros (ações, títulos, cripto, 350+ bases) para análise, com SDK em Python e integração com agentes de IA. |

---

## 9. Documentos e assinatura

| Ferramenta | Licença | O que faz |
|---|---|---|
| [DocuSeal](https://github.com/docusealco/docuseal) | AGPL-3.0 + termos adicionais (recursos Pro pagos) | Cria PDFs preenchíveis e coleta assinatura digital. Alternativa básica ao DocuSign. |
| [Paperless-ngx](https://github.com/paperless-ngx/paperless-ngx) | GPL-3.0 | Digitaliza papéis e vira um arquivo pesquisável online (OCR, etiquetas, busca). |
| [Gotenberg](https://github.com/gotenberg/gotenberg) | MIT | API em Docker que converte HTML, Markdown e documentos do Office em PDF. Útil pra gerar relatórios e faturas em automações. |
| [Chandra](https://github.com/datalab-to/chandra) | Apache-2.0 (conferir a licença do modelo) | OCR com IA que lê imagem/PDF e devolve Markdown/HTML mantendo layout, tabelas, escrita à mão e 90+ idiomas. |

---

## 10. Produtividade e conhecimento

| Ferramenta | Licença | O que faz |
|---|---|---|
| [AFFiNE](https://github.com/toeverything/AFFiNE) | ⚠️ Licença própria (conferir) | Documentos, quadro branco e bancos de dados num lugar só. Alternativa ao Notion + Miro. |
| [SiYuan](https://github.com/siyuan-note/siyuan) | AGPL-3.0 | Anotações em blocos com links entre notas (tipo Obsidian/Notion), local-first. |
| [BookStack](https://github.com/BookStackApp/BookStack) | MIT | Wiki pra documentação interna e de entrega ao cliente. |
| [Outline](https://getoutline.com) | ⚠️ BSL | Wiki bonita, mas licença restritiva. |
| [Super Productivity](https://github.com/super-productivity/super-productivity) | MIT | Lista de tarefas com cronômetro, pomodoro e controle de horas. Integra com Jira/GitHub/GitLab. |
| [linkding](https://github.com/sissbruecker/linkding) | MIT | Gerenciador de favoritos com tags, notas e arquivo da página. Biblioteca de pesquisa compartilhada. |
| [Snipe-IT](https://github.com/snipe/snipe-it) | AGPL-3.0 | Controle de equipamentos de TI: quem está com o quê, compras e licenças de software. |
| [Vaultwarden](https://github.com/dani-garcia/vaultwarden) | AGPL-3.0 | Servidor de senhas compatível com o app Bitwarden. Cofres por cliente. |

---

## 11. E-commerce

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Medusa](https://github.com/medusajs/medusa) | MIT | Plataforma de loja virtual modular: pedidos, estoque, preços, promoções, várias moedas e regiões. Alternativa ao Shopify/Magento para quem quer loja sob medida. |

---

## 12. Autenticação e identidade

| Ferramenta | Licença | O que faz |
|---|---|---|
| [ZITADEL](https://github.com/zitadel/zitadel) | AGPL-3.0 (algumas partes Apache/MIT) | Sistema de login completo: SSO, MFA, passkeys, vários clientes (multi-tenant) e trilha de auditoria. Alternativa ao Auth0/Okta. |
| [Stack Auth](https://github.com/stack-auth/stack-auth) | MIT e AGPL-3.0 (licença dupla) | Login pronto pra app: OAuth, senha, link mágico, passkeys, times e painel de usuários. Alternativa ao Clerk/Auth0. |

---

# DEV E INFRAESTRUTURA

## 13. Sites, CMS, backend e armazenamento

### 13.1 Sites e CMS

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Payload CMS](https://github.com/payloadcms/payload) | MIT | CMS com painel de admin que roda dentro do seu app Next.js. Um repositório só por cliente. |
| [Astro](https://github.com/withastro/astro) | MIT | Framework pra sites rápidos focados em conteúdo e landing pages. |
| [Strapi](https://github.com/strapi/strapi) | MIT + Enterprise pago | CMS com painel e API pronta, muito conhecido. |
| [Ghost](https://github.com/TryGhost/Ghost) | MIT | Blog + newsletter + membros prontos. |
| [Puck](https://github.com/puckeditor/puck) | MIT | Editor visual arrastar-e-soltar sobre seus componentes React. Vira um "construtor de páginas" pro cliente. |
| [GrapesJS](https://github.com/GrapesJS/grapesjs) | BSD-3 | Base pra criar editor visual de páginas ou e-mails. |
| [Directus](https://directus.io) | ⚠️ MSCL | CMS/painel que transforma um banco SQL existente em API e admin. Grátis só abaixo de US$ 5M de receita e 50 funcionários (versão 12 em diante). |

### 13.2 Backends, bancos e armazenamento

| Ferramenta | Licença | O que faz |
|---|---|---|
| [PocketBase](https://github.com/pocketbase/pocketbase) | MIT | Backend inteiro num arquivo só: banco, login, upload e painel. Ideal pra MVP. |
| [Supabase](https://github.com/supabase/supabase) | Apache-2.0 | Backend completo sobre Postgres (login, storage, tempo real). Pesado pra self-host. |
| [Appwrite](https://github.com/appwrite/appwrite) | BSD-3 | Alternativa ao Supabase, instalação Docker simples. |
| [Baserow](https://github.com/bram2w/baserow) | MIT (núcleo) | Planilha-banco estilo Airtable. |
| [NocoDB](https://nocodb.com) | ⚠️ Sustainable Use License (desde jan/2026) | Estilo Airtable; agora só pra uso interno. Prefira Baserow. |
| [MinIO](https://github.com/minio/minio) | AGPL-3.0 (opção comercial) | Armazenamento de arquivos compatível com o S3 da Amazon, no seu servidor. Pra backups e mídia. |
| [Databasus](https://github.com/databasus/databasus) | Apache-2.0 | Backup automático de bancos (PostgreSQL, MySQL, MongoDB) com agendamento, criptografia e envio pra S3/Drive/FTP. |
| [Supavisor](https://github.com/supabase/supavisor) | Apache-2.0 | Gerencia conexões com o Postgres (connection pooler), pra o banco não travar com muitos acessos. |
| [Refine](https://github.com/refinedev/refine) | MIT | Framework React pra sistemas admin/CRUD: login, permissões, conexão com qualquer API. O melhor pra sistemas internos. |

---

## 14. Infraestrutura, deploy e hospedagem

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Coolify](https://github.com/coollabsio/coolify) | Apache-2.0 | "Vercel/Heroku próprio": faz deploy de apps em várias VPS com SSL automático, e tem 280+ serviços prontos de um clique. |
| [Dokploy](https://github.com/Dokploy/dokploy) | Apache-2.0 (núcleo) + ⚠️ parte proprietária | Alternativa ao Coolify. SSO, permissões e white-label são pagos. |
| [Portainer CE](https://github.com/portainer/portainer) | zlib | Interface web pra gerenciar containers Docker. |
| [Caddy](https://github.com/caddyserver/caddy) | Apache-2.0 | Proxy reverso com HTTPS automático, o mais simples de manter. |
| [Restic](https://github.com/restic/restic) | BSD-2 | Backup incremental e criptografado pra S3/B2. Sem backup, o resto é risco. |
| [Cloudflare Pages](https://pages.cloudflare.com) | Freemium (banda ilimitada, 500 builds/mês) | Hospeda sites estáticos de graça, inclusive comerciais. |
| [Netlify](https://netlify.com) | Freemium (300 créditos/mês, ~15 GB) | Hospedagem de sites com deploy automático. |
| [GitHub Pages](https://pages.github.com) | Grátis (100 GB/mês, site até 1 GB) | Hospeda sites estáticos direto do repositório. |
| [Vercel Hobby](https://vercel.com) | Freemium (100 GB) ⚠️ | Hospedagem ótima pra Next.js, mas o plano grátis proíbe uso comercial. |

---

## 15. Testes e segurança

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Playwright](https://github.com/microsoft/playwright) | Apache-2.0 | Testes automáticos de ponta a ponta no navegador. Também compara prints (`toHaveScreenshot()`) pra pegar mudança visual sem querer. |
| [Bruno](https://github.com/usebruno/bruno) | MIT | Testa APIs, com coleções salvas no repositório. Substitui o Postman. |
| [Yaade](https://github.com/EsperoTech/yaade) | MIT | Ambiente de testes de API colaborativo e self-hosted (alternativa ao Postman). Vários usuários, importa de Postman/OpenAPI. |
| [k6](https://github.com/grafana/k6) | AGPL-3.0 | Teste de carga: descobre se o servidor aguenta um pico. |
| [Trivy](https://github.com/aquasecurity/trivy) | Apache-2.0 | Procura vulnerabilidades em imagens Docker e dependências. |
| [Gitleaks](https://github.com/gitleaks/gitleaks) | MIT | Impede que senhas e chaves vazem no git. |
| [SonarQube Community](https://github.com/SonarSource/sonarqube) | LGPL-3.0 | Análise de qualidade do código, com relatório. |
| [OpenCTI](https://github.com/OpenCTI-Platform/opencti) | ⚠️ Licença própria estilo Apache-2.0 (conferir) | Plataforma de inteligência de ameaças cibernéticas: reúne indicadores, vulnerabilidades e relatórios num grafo. Só faz sentido se você oferecer segurança como serviço. |

---

## 16. Monitoramento e observabilidade

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Uptime Kuma](https://github.com/louislam/uptime-kuma) | MIT | Avisa quando um site cai (HTTP, ping, DNS, Docker...) e gera página de status. 90+ canais de aviso. Fácil de vender como "monitoramento 24/7". |
| [Kener](https://github.com/rajnandan1/kener) | MIT | Página de status bonita e leve, com monitoramento, histórico de uptime e gestão de incidentes. |
| [OpenStatus](https://github.com/openstatusHQ/openstatus) | AGPL-3.0 | Página de status + monitoramento de uptime e de APIs a partir de várias regiões. Alternativa ao StatusPage/Better Uptime. |
| [Gatus](https://github.com/TwiN/gatus) | Apache-2.0 | Checagens de saúde configuradas em arquivo (YAML) + página de status. |
| [Beszel](https://github.com/henrygd/beszel) | MIT | Painel leve de CPU, RAM, disco e containers de várias VPS, com alertas. |
| [GlitchTip](https://gitlab.com/glitchtip/glitchtip) | MIT | Captura erros do app (compatível com Sentry) usando pouca memória (~512 MB). |
| [OpenObserve](https://github.com/openobserve/openobserve) | AGPL-3.0 | Logs, métricas, traces e monitoramento de front-end num lugar só, em um único binário. Alternativa barata ao Datadog/Splunk. |
| [Uptrace](https://github.com/uptrace/uptrace) | ⚠️ Licença própria (conferir) | Monitoramento de performance (APM) com OpenTelemetry: traces, métricas e logs numa tela. |
| [Grafana](https://github.com/grafana/grafana) + [Loki](https://github.com/grafana/loki) | AGPL-3.0 | Dashboards e logs centralizados. |
| [Prometheus](https://prometheus.io) | Apache-2.0 | Coleta métricas dos servidores e apps. |
| [Sentry self-hosted](https://github.com/getsentry/self-hosted) | ⚠️ FSL | Captura de erros completa, mas exige 16+ GB de RAM e proíbe oferecer como serviço. Use GlitchTip. |

---

## 17. Produtividade de dev

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Plane](https://github.com/makeplane/plane) | AGPL-3.0 | Gestão de projetos estilo Jira/Linear (sprints, quadros, Gantt), pra acompanhar entregas com clientes. |
| [Gitea](https://github.com/go-gitea/gitea) | MIT | GitHub próprio, com CI (Actions). |
| [Gogs](https://github.com/gogs/gogs) | MIT | Git self-hosted mais simples e leve que o Gitea (um binário só). Gitea nasceu como fork dele. |
| [Woodpecker CI](https://github.com/woodpecker-ci/woodpecker) | Apache-2.0 | CI/CD leve baseado em containers. |
| [Infisical](https://github.com/Infisical/infisical) | MIT + Enterprise pago | Guarda senhas e variáveis de ambiente de todos os clientes e injeta no deploy. |
| [GitNexus](https://github.com/abhigyanpatwari/GitNexus) | ⚠️ Licença própria (conferir) | Joga um repositório no navegador e ele gera um mapa interativo do código, com agente de IA que responde dúvidas. Tudo local, sem servidor. |
| [Archon](https://github.com/coleam00/Archon) | MIT | Define o processo de desenvolvimento com IA em arquivos YAML (planejar, implementar, validar, revisar) pra o agente repetir sempre a mesma sequência. |

---

## 18. IA

### 18.1 Agentes, apps e interfaces de chat

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Paperclip](https://github.com/paperclipai/paperclip) | MIT | Organiza agentes de IA (Claude Code, Codex) como uma "empresa", com cargos, orçamento e regras. Projeto novo, muda rápido. |
| [Dify](https://github.com/langgenius/dify) | ⚠️ Apache-2.0 com termos adicionais (conferir antes de revender) | Monta apps e fluxos de IA num canvas visual: 200+ modelos, base de conhecimento (RAG), agentes e API. |
| [LibreChat](https://github.com/danny-avila/LibreChat) | MIT | "ChatGPT da empresa" com vários modelos, agentes e MCP; pode ter a marca do cliente. |
| [Onyx](https://github.com/onyx-dot-app/onyx) | MIT (recursos enterprise à parte) | Chat de IA que busca nos documentos da empresa: 40+ conectores, agentes e pesquisa profunda. |
| [Open WebUI](https://openwebui.com) | ⚠️ Licença própria | Interface de chat pra Ollama/OpenAI com RAG. Acima de 50 usuários não pode tirar a marca. Pra white-label, use LibreChat. |
| [Ollama](https://github.com/ollama/ollama) | MIT | Roda modelos de IA no seu computador/servidor, pra dados sensíveis. |
| [OpenWork](https://github.com/different-ai/openwork) | ⚠️ Termos próprios (conferir) | Alternativa open source ao Claude Cowork: app desktop onde agentes de IA executam tarefas, com conectores (WhatsApp, Slack, Telegram). |
| [Airi](https://github.com/moeru-ai/airi) | MIT | Companheiro de IA com voz, que joga (Minecraft) e tem personalidade configurável. Rodando local. |

### 18.2 Memória, observabilidade e dados para IA

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Langfuse](https://github.com/langfuse/langfuse) | MIT + Enterprise pago | Mostra custo, tempo e qualidade de cada chamada de IA dos seus agentes. |
| [Mem0](https://github.com/mem0ai/mem0) | Apache-2.0 | Camada de memória de longo prazo pra assistentes de IA lembrarem de usuários e conversas anteriores. |
| [OpenViking](https://github.com/volcengine/OpenViking) | Apache-2.0 | Banco de contexto pra agentes: organiza memória, recursos e skills como se fossem pastas e arquivos. |
| [MCP servers oficiais](https://github.com/modelcontextprotocol/servers) | MIT (conferir cada um) | Ferramentas prontas pro Claude Code (arquivos, git, fetch). |

### 18.3 IA para código

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Continue](https://github.com/continuedev/continue) | Apache-2.0 | Assistente de código aberto (IDE/CLI) que aceita modelos locais. |
| [Tabby](https://github.com/TabbyML/tabby) | ⚠️ Licença própria (conferir) | Autocompletar de código com IA no seu servidor (VS Code, JetBrains, Vim), alternativa ao Copilot. |

### 18.4 IA para finanças e voz

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Dexter](https://github.com/virattt/dexter) | MIT | Agente que pesquisa e analisa finanças sozinho: lê balanços, planeja a análise e confere o próprio resultado. |
| [Kronos](https://github.com/shiyu-coder/Kronos) | MIT | Modelo de IA treinado em gráficos de candlestick de 45+ bolsas, pra análise e previsão de mercado. |
| [Voicebox](https://github.com/jamiepine/voicebox) | MIT | Estúdio de voz local: clona uma voz com poucos segundos de áudio e gera fala em 23 idiomas. Alternativa ao ElevenLabs. |

---

## 19. Utilitários e outros

| Ferramenta | Licença | O que faz |
|---|---|---|
| [frp](https://github.com/fatedier/frp) | Apache-2.0 | Túnel próprio (tipo ngrok) pra expor webhooks locais pela sua VPS. |
| [ntfy](https://github.com/binwiederhier/ntfy) | Apache-2.0 / GPL-2.0 | Manda notificações pro celular via HTTP (alerta de deploy, erro). |
| [Meilisearch CE](https://github.com/meilisearch/meilisearch) | MIT (Community) | Busca instantânea tipo Algolia. A versão Enterprise é paga. |
| [BullMQ](https://github.com/taskforcesh/bullmq) | MIT | Filas de tarefas em segundo plano (Node + Redis). |
| [Unleash](https://github.com/Unleash/unleash) | Apache-2.0 | Feature flags: liga/desliga recursos por cliente. |
| [Scalar](https://github.com/scalar/scalar) | MIT | Documentação bonita e interativa de API. |
| [Mockoon](https://github.com/mockoon/mockoon) | MIT | Simula uma API pra fazer o front antes do backend existir. |
| [lazydocker](https://github.com/jesseduffield/lazydocker) | MIT | Painel no terminal pra debugar containers. |
| [Fastfetch](https://github.com/fastfetch-cli/fastfetch) | MIT | Mostra informações do sistema no terminal (versão rápida e mantida do neofetch). |
| [Project N.O.M.A.D](https://github.com/Crosstalk-Solutions/project-nomad) | Apache-2.0 | "Computador de sobrevivência" offline com IA local, guias, mapas e ferramentas de emergência. Roda em Raspberry Pi ou notebook. |

---

# DESIGN E FRONT-END

## 20. Design

### 20.1 Ferramentas de design

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Penpot](https://github.com/penpot/penpot) | MPL-2.0 | Alternativa ao Figma, web e self-hosted. |
| [Excalidraw](https://github.com/excalidraw/excalidraw) | MIT | Quadro branco com cara de rascunho, pra wireframes e reuniões. |
| [draw.io](https://github.com/jgraph/drawio) | Apache-2.0 | Diagramas técnicos e fluxogramas. |

*(AFFiNE, que também faz quadro branco, está na seção 10.)*

### 20.2 Cores e design tokens

| Ferramenta | Licença | O que faz |
|---|---|---|
| Tailwind v4 `@theme` | MIT | Define cores, fontes e espaçamentos num lugar só e gera as classes. |
| [Style Dictionary](https://styledictionary.com) | Apache-2.0 | Converte tokens de design pra CSS, Tailwind, mobile etc. Só vale com mais de um destino. |
| [Tokens Studio](https://tokens.studio) | Freemium (Starter grátis) | Plugin do Figma que sincroniza tokens com o Git. |
| [Tweakcn](https://tweakcn.com) | Open source | Editor visual de tema para shadcn (cores, raio, fontes). Tira a "cara de shadcn" do app. |
| [Harmonizer](https://harmonizer.evilmartians.com) | Open source | Gera paletas de cor com contraste consistente (inclui dark mode) e exporta pra Tailwind. |
| [oklch.com](https://oklch.com) | Grátis | Seletor de cor no formato OKLCH. |
| Polychrom / apcach | Open source | Checa contraste de texto (APCA) no Figma / gera cor pelo contraste desejado. |
| [Adobe Leonardo](https://leonardocolor.io) | Grátis | Escalas de cor baseadas em contraste. |
| [Radix Colors](https://github.com/radix-ui/colors) | MIT | Escalas de cor acessíveis prontas. |
| [Realtime Colors](https://realtimecolors.com) | Grátis | Testa sua paleta num site de exemplo na hora. |
| [Coolors](https://coolors.co) | Freemium | Gera e explora paletas. |
| MantineHub | Grátis | Gerador de temas para Mantine. |

### 20.3 Design systems (documentar componentes)

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Storybook](https://github.com/storybookjs/storybook) | MIT | Catálogo navegável dos seus componentes, pra documentar e entregar ao cliente. |
| [Ladle](https://github.com/tajo/ladle) | MIT | Storybook leve para React. |
| [Histoire](https://github.com/histoire-dev/histoire) | MIT | Storybook leve para Vue/Svelte. |

### 20.4 Ícones

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Lucide](https://github.com/lucide-icons/lucide) | ISC | Ícones padrão do shadcn. |
| [Tabler Icons](https://github.com/tabler/tabler-icons) | MIT | 5.000+ ícones em traço, ótimo pra dashboards. |
| [Phosphor](https://phosphoricons.com) | MIT | Ícones em 6 pesos, visual mais "de marca". |
| [Heroicons](https://github.com/tailwindlabs/heroicons) | MIT | Ícones do time do Tailwind. |
| [Iconify](https://iconify.design) | Grátis | Uma API só pra acessar dezenas de coleções de ícones. |
| [Font Awesome Free](https://github.com/FortAwesome/Font-Awesome) | ⚠️ CC BY 4.0 (exige atribuição) | Ícones populares; prefira Lucide/Tabler pra não precisar creditar. |

### 20.5 Fontes

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Google Fonts](https://fonts.google.com) | OFL (maioria) | Catálogo grande de fontes livres. Hospede os arquivos você mesmo (melhor pra RGPD). |
| [Fontsource](https://fontsource.org) | Varia (maioria OFL) | Instala fontes via npm pra self-host. |
| [Fontshare](https://fontshare.com) | Grátis, uso comercial | Fontes com cara premium, sem atribuição. |
| [Inter](https://rsms.me/inter) / [Geist](https://vercel.com/font) | OFL | Fontes de interface muito usadas. |

### 20.6 Fotos, imagem e vídeo

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Unsplash API](https://unsplash.com/developers) | Freemium (50 req/h; 5.000 após aprovação) | Fotos grátis via API. |
| [Pexels API](https://pexels.com/api) | Grátis (200 req/h, 20.000/mês) | Fotos e vídeos grátis via API. |
| [rembg](https://github.com/danielgatis/rembg) | MIT | Remove fundo de imagens automaticamente. |
| [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | GPL-3.0 | Gera imagens com IA em fluxos de nós, no seu computador. Atenção à licença de cada modelo. |
| [Satori](https://github.com/vercel/satori) | MPL-2.0 | Gera imagens de compartilhamento (OG image) a partir de HTML/JSX. |
| [FFmpeg](https://ffmpeg.org) | LGPL/GPL | Corta, converte e gera miniaturas de vídeo/áudio por comando. |
| [Kdenlive](https://kdenlive.org) | GPL | Editor de vídeo desktop. |
| [Remotion](https://github.com/remotion-dev/remotion) | ⚠️ Licença própria | Cria vídeos programando em React. Grátis pra indivíduos/empresas pequenas; empresas maiores pagam. |

---

## 21. Front-end: componentes e interface

### 21.1 Primitives (a base "sem estilo" dos componentes)

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Base UI](https://base-ui.com) | MIT | Componentes acessíveis sem estilo (menus, diálogos, combobox). Padrão novo do shadcn. Primeira escolha em projeto novo. |
| [Radix UI](https://radix-ui.com) | MIT | Mesma ideia do Base UI, mais antigo e maduro. |
| [React Aria (Adobe)](https://react-spectrum.adobe.com/react-aria) | Apache-2.0 | O melhor em acessibilidade e internacionalização (datas, calendários, arrastar). |
| [Ark UI](https://ark-ui.com) | MIT | Primitives que funcionam em React, Vue, Solid e Svelte. |

### 21.2 Kits de componentes prontos

| Ferramenta | Licença | O que faz |
|---|---|---|
| [shadcn/ui](https://github.com/shadcn-ui/ui) | MIT | Componentes que você copia pro projeto (o código fica seu). O Claude Code domina. |
| [Mantine](https://mantine.dev) | MIT | Biblioteca React completa (formulários, datas, gráficos). Ótima pra painéis internos. |
| [daisyUI](https://daisyui.com) | MIT | Componentes em classes Tailwind, funciona em qualquer framework. |
| [Nuxt UI](https://ui.nuxt.com) | MIT | Componentes para Vue/Nuxt. |
| [shadcn-svelte](https://github.com/huntabyte/shadcn-svelte) | MIT | shadcn para Svelte. |
| [coss ui (ex-Origin UI)](https://coss.com/ui) | ⚠️ Conferir (raiz AGPL, apps de UI MIT) | Design system do Cal.com: centenas de componentes de aplicação sem firula. |
| [Kokonut UI](https://kokonutui.com) | MIT | Componentes modernos e animados para shadcn. |
| [Magic UI](https://magicui.design) | MIT (parte grátis) | 150+ microinterações e seções animadas para landing pages. |
| [Aceternity UI](https://ui.aceternity.com) | ⚠️ Licença própria | Heroes e efeitos "cinematográficos". Uso comercial liberado, mas proibido revender os componentes. |
| [21st.dev](https://21st.dev) | Varia por autor | Marketplace comunitário de componentes shadcn. Bom pra descobrir; confira a licença de cada item. |
| [registry.directory](https://registry.directory) | Grátis | Diretório pra achar outras coleções baseadas em shadcn. |

### 21.3 Dashboards e sistemas

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Tremor](https://tremor.so) | MIT | Componentes de gráficos e dashboards (React + Tailwind), com 300 blocos prontos. |
| [React Admin](https://marmelab.com/react-admin) | MIT | Alternativa madura ao Refine (seção 13.2), visual estilo Material. |
| [shadcn-admin](https://github.com/satnaing/shadcn-admin) | MIT | Template de painel admin com 10+ páginas prontas. |
| [next-shadcn-dashboard-starter](https://github.com/Kiranism/next-shadcn-dashboard-starter) | MIT | Ponto de partida pra SaaS em Next.js com tabelas, formulários e login. |

### 21.4 Tabelas, formulários e gráficos

| Ferramenta | Licença | O que faz |
|---|---|---|
| [TanStack Table](https://tanstack.com/table) | MIT | Lógica de tabela (ordenar, filtrar, paginar) sem visual. Você monta a UI. |
| [AG Grid Community](https://ag-grid.com) | MIT | Tabela completa que aguenta milhões de linhas. Agrupamento e export Excel são pagos. |
| [react-data-grid](https://github.com/adazzle/react-data-grid) | MIT | Tabela editável estilo planilha, mais leve. |
| [TanStack Form](https://tanstack.com/form) / [React Hook Form](https://react-hook-form.com) | MIT | Gerenciam formulários no React. |
| [Zod](https://zod.dev) | MIT | Valida dados (ex.: "e-mail obrigatório, idade > 18"). |
| [Recharts](https://recharts.org) | MIT | Gráficos simples em React (base do Tremor e dos charts do shadcn). |
| [Apache ECharts](https://echarts.apache.org) | Apache-2.0 | Gráficos pesados e interativos. |
| [visx](https://airbnb.io/visx) | MIT | Peças do D3 em React pra gráficos sob medida. |

### 21.5 Texto e tipografia

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Pretext](https://github.com/chenglou/pretext) | MIT | Calcula altura e quebra de linha de texto sem renderizar. Útil em chat com streaming, listas virtualizadas e canvas. Exagero pra site comum. |
| CSS `text-wrap: balance` / `pretty` | Nativo | Equilibra linhas de títulos e evita palavra sozinha no fim do parágrafo, sem JS. |
| CSS `clamp()` + container queries | Nativo | Fonte que cresce e encolhe conforme a tela ou o bloco onde está. |

### 21.6 Recursos nativos do CSS/navegador (sem biblioteca)

| Recurso | Licença | O que faz |
|---|---|---|
| Anchor Positioning + Popover API | Nativo | Tooltips e menus presos ao botão sem biblioteca. |
| View Transitions | Nativo | Transição animada entre telas/estados. |
| Scroll-driven animations | Nativo (sem Firefox) | Animações que acompanham a rolagem, sem JS. |

### 21.7 Backgrounds e efeitos visuais

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Paper Shaders](https://shaders.paper.design) | Apache-2.0 | Fundos animados leves e profissionais: mesh gradient, granulado, metal líquido. |
| [React Bits](https://reactbits.dev) | ⚠️ MIT + Commons Clause | Maior catálogo grátis de fundos animados (Liquid Chrome, Aurora, Silk...). Pode usar comercialmente, não pode revender os componentes. |
| [ShaderGradient](https://shadergradient.co) | Grátis | Gradientes 3D em movimento estilo Stripe/Apple. Pesado (usa three.js). |
| [tsParticles](https://particles.js.org) | MIT | Partículas, confete e efeitos que reagem ao mouse. |
| [OGL](https://github.com/oframe/ogl) | Unlicense | Base mínima de WebGL pra escrever seus próprios efeitos leves. |
| [three.js](https://threejs.org) | MIT | 3D completo no navegador. |
| [React Three Fiber](https://github.com/pmndrs/react-three-fiber) | MIT | three.js escrito como componentes React. |
| [Vanta.js](https://vantajs.com) | MIT | Fundos 3D animados. Parado desde 2022: evite em projeto novo. |

### 21.8 Animação

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Motion (ex-Framer Motion)](https://motion.dev) | MIT | Animações em React: entradas, saídas, gestos, layout. Padrão pra apps. |
| [GSAP](https://gsap.com) | Licença própria, 100% grátis (inclusive comercial) | Animações complexas com rolagem, texto dividido, morph de SVG. Padrão pra landing pages "premiadas". |
| [AutoAnimate](https://auto-animate.formkit.com) | MIT | Uma linha de código pra animar listas que entram, saem ou mudam de ordem. |
| [Lenis](https://github.com/darkroomengineering/lenis) | MIT | Rolagem suave, visual "site premium". |
| [Anime.js](https://animejs.com) | MIT | Motor de animação leve. |
| [lottie-web](https://github.com/airbnb/lottie-web) | MIT | Toca animações feitas por designers (Lottie) sem vídeo pesado. |

---

## 22. Ajuste visual com IA (localhost)

### 22.1 Apontar elemento da tela pra IA

| Ferramenta | Licença | O que faz |
|---|---|---|
| [react-grab](https://github.com/aidenybai/react-grab) | MIT | Passa o mouse num elemento, aperta ⌘C e cola no Claude Code o arquivo e a linha exatos. |
| [Agentation](https://agentation.com) | ⚠️ PolyForm Shield (grátis pra uso interno) | Clica e anota vários detalhes da página de uma vez e manda tudo pro agente como lista. |
| [Vercel Toolbar – Copy for Agents](https://vercel.com/changelog/copy-visual-context-to-agents) | Grátis (usuários Vercel) | Copia contexto de um elemento num preview da Vercel pra colar no agente. |
| [ide-byebye](https://github.com/bo-516/ide-byebye) | Open source (experimental) | ⌘-clique num elemento abre o agente já com arquivo e pedido. |

### 22.2 Clicar na tela e abrir o código

| Ferramenta | Licença | O que faz |
|---|---|---|
| [code-inspector-plugin](https://inspector.fe-dev.cn/en) | MIT | Clica num elemento e abre o arquivo exato no editor. Funciona com Next/Turbopack e Vue. |
| [LocatorJS](https://locatorjs.com) | Open source | Mesma ideia; ainda com problemas no React 19. |
| [@stinsky/xray](https://github.com/ivanstnsk/xray) | Open source | Mostra nome do componente e arquivo ao passar o mouse. |

### 22.3 Editores visuais que gravam no código

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Cursor Browser Visual Editor](https://cursor.com/blog/browser-visual-editor) | Freemium (Cursor Free com limites de IA) | Arrasta elementos e ajusta espaçamento/cor com sliders, e grava no código. |
| [Onlook](https://github.com/onlook-dev/onlook) | Apache-2.0 | Edição estilo Figma em cima do seu repositório Next.js + Tailwind. Instável. |
| [Stagewise](https://stagewise.io) | AGPL-3.0 (Hobby grátis) | IDE com navegador próprio onde o agente vê console e DOM. Ainda alpha. |
| [Chrome DevTools AI + Workspaces](https://developer.chrome.com/docs/devtools/ai-assistance) | Grátis | Edita CSS no DevTools e salva no arquivo. Fraco pra classes Tailwind. |
| [Subframe](https://subframe.com) | Freemium (1 projeto) | Desenha componentes num canvas e gera código React + Tailwind. |

### 22.4 IA vendo o navegador (MCP)

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp) | Open source | Deixa o agente abrir a página, tirar print, ler o console e rodar Lighthouse. Fecha o ciclo "a IA confere o próprio ajuste". |
| [Playwright MCP](https://github.com/microsoft/playwright-mcp) | Open source | Agente dirige o navegador: clica, preenche formulários, testa fluxos. |
| [agent-browser (Vercel Labs)](https://github.com/vercel-labs/agent-browser) | Open source | Navegador pra agentes que gasta bem menos contexto que o Playwright MCP. |

### 22.5 Comparar com o design (pixel-perfect)

| Ferramenta | Licença | O que faz |
|---|---|---|
| [Mockpup](https://mockpup.com) | Grátis | Sobrepõe o design do Figma na página e mostra as diferenças. |
| PerfectPixel | Grátis (com limites) | Overlay de imagem do design sobre o site. |
| PixelParallel | Grátis | Overlay + grade de colunas + réguas. |

*(Comparação automática de prints: ver Playwright na seção 15.)*

---

## 23. Skills e recursos anti-"cara de IA"

| Ferramenta | Licença | O que faz |
|---|---|---|
| [frontend-design SKILL.md](https://github.com/anthropics/skills) | Open source | Instruções da Anthropic pro Claude fazer interface com personalidade, não genérica. |
| [Frontend Aesthetics Cookbook](https://github.com/anthropics/claude-cookbooks) | Grátis | Exemplos de prompt pra evitar o visual "feito por IA". |
| [Unslop UI](https://github.com/JCarterJohnson/vibecoded-design-tells) | MIT | Lista dos sinais de "site feito por IA" + scanner que roda no CI. |
| [landing-page-design](https://github.com/2389-research/landing-page-design) | Grátis | Processo guiado pra definir estilo e texto de landing page antes de codar. |
| [OneRedOak design-review](https://github.com/OneRedOak/claude-code-workflows) | MIT | Subagente que revisa o design abrindo a página no navegador. |
| [Vercel Web Interface Guidelines](https://github.com/vercel-labs/web-interface-guidelines) | Grátis | Checklist que o agente segue e audita: foco, teclado, formulários, animação, dark mode. |
| [extract-design-system](https://github.com/arvindrk/extract-design-system) | Grátis | Extrai cores, fontes e espaçamentos de um site pronto. |
| [designlang (design-extract)](https://github.com/Manavarya09/design-extract) | Grátis | Transforma um site em DESIGN.md + tema Tailwind. |
| [design.md (Google Labs)](https://github.com/google-labs-code/design.md) | Apache-2.0 | Padrão de arquivo DESIGN.md pra descrever o design do projeto pra IA. |
| [claude-design-mcp](https://github.com/Evilander/claude-design-mcp) | Grátis | Gera várias variações de tela em paralelo, com prints. |

---

## 24. Qualidade de UI: linters, acessibilidade e performance

| Ferramenta | Licença | O que faz |
|---|---|---|
| [eslint-plugin-better-tailwindcss](https://www.npmjs.com/package/eslint-plugin-better-tailwindcss) | MIT | Bloqueia classes Tailwind fora do seu tema e cores "chutadas" (`bg-[#ff0000]`). |
| oxlint-tailwindcss | Open source | Mesma ideia, para quem usa oxlint. |
| [eslint-plugin-jsx-a11y](https://github.com/jsx-eslint/eslint-plugin-jsx-a11y) | MIT | Aponta erros de acessibilidade no JSX antes do deploy. |
| [axe-core](https://github.com/dequelabs/axe-core) | MPL-2.0 | Motor de teste de acessibilidade; integra com Playwright. |
| axe DevTools / WAVE | Grátis (extensões) | Checam contraste, foco e ARIA na página aberta. |
| [Pa11y](https://github.com/pa11y/pa11y) | LGPL-3.0 | Relatório de acessibilidade por linha de comando. |
| [Accessibility Insights](https://github.com/microsoft/accessibility-insights-web) | MIT | Extensão que guia uma auditoria manual de acessibilidade. |
| [Lighthouse CI](https://github.com/GoogleChrome/lighthouse-ci) | Apache-2.0 | Roda o Lighthouse a cada deploy e guarda o histórico. Bom pra mostrar "antes/depois". |
| [sitespeed.io](https://github.com/sitespeedio/sitespeed.io) | MIT | Monitora a performance do site ao longo do tempo. |
| [web-vitals](https://github.com/GoogleChrome/web-vitals) | Apache-2.0 | Coleta a velocidade real que os visitantes sentem (LCP, INP, CLS). |
| [sharp](https://github.com/lovell/sharp) | Apache-2.0 | Converte e redimensiona imagens (AVIF/WebP) no build. |
| [imgproxy](https://github.com/imgproxy/imgproxy) | MIT | Servidor que redimensiona imagens na hora. CDN de imagens própria. |
| [Squoosh](https://squoosh.app) | Open source | Comprime imagens no navegador, uma a uma. |

---

## 25. Referências de estudo e inspiração

| Recurso | O que é |
|---|---|
| [interfaces.rauno.me](https://interfaces.rauno.me) | Detalhes de microinteração, estados, inputs e foco. |
| [joshwcomeau.com](https://joshwcomeau.com) | Artigos sobre CSS, sombras e foco, muito didáticos. |
| [Laws of UX](https://lawsofux.com) | Princípios de UX explicados de forma curta. |
| Vercel Geist, GitHub Primer, Atlassian, Radix Themes | Design systems públicos pra copiar decisões (raio, sombra, densidade). |
| Tremor Blocks, shadcn Blocks | Blocos de tela prontos e grátis. |
| [Godly](https://godly.website), [Land-book](https://land-book.com), [Awwwards](https://awwwards.com) | Galerias de sites pra referência visual. |

---

## Fora da lista (só pagas, só trial ou sem valor no grátis)

Pipedrive, Folk, LinkedIn Sales Navigator, RocketReach, Cal.com (fechou o código em abr/2026; use Cal.diy), Unicorn Studio (grátis só pra uso pessoal), Spline (grátis com marca d'água), Builder.io Fusion, Tempo Labs, Codux, Over.fig, versões Pro/pagas (Motion+, Magic UI Pro, Aceternity All-Access, React Bits Pro, AG Grid Enterprise), cursos pagos (animations.dev, Refactoring UI) e Warmbly (licença não confirmada).
