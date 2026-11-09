# 💊 Fale com o Farmacêutico

Conceito de funcionalidade para **farmácias em apps de delivery**: um canal para o cliente tirar dúvidas com o **farmacêutico responsável da loja** antes de comprar.

> Protótipo de interface (UX/produto) — não é um produto oficial nem tem vínculo com nenhuma empresa.

**▶️ Ver o protótipo:** abra o [`index.html`](index.html) no navegador ou acesse a versão publicada no GitHub Pages.

---

## O problema

Quem compra em uma farmácia física pode perguntar ao balcão: *"posso tomar isso junto com meu remédio de pressão?"*. No delivery, essa conversa some.

- O cliente compra sem orientação ou desiste da compra por insegurança.
- A farmácia perde o seu maior diferencial, que é ter um profissional habilitado.
- O farmacêutico, obrigatório em toda farmácia, fica fora da jornada digital.

## A proposta

Um botão **"Falar com o farmacêutico"** dentro da loja de cada farmácia, que abre um chat com o profissional responsável.

| Tela | O que acontece |
|---|---|
| **1 · Loja** | Card de destaque com o status "farmacêutico disponível", o botão "Tirar dúvida" em cada produto e um atalho flutuante. |
| **2 · Antes da conversa** | Triagem rápida: o tema da dúvida, os medicamentos em uso (opcional), o consentimento LGPD e um aviso de emergência (SAMU 192). |
| **3 · Chat** | O farmacêutico aparece identificado por nome e CRF, recebe um resumo da triagem e pode sugerir um produto, que o cliente adiciona à sacola direto pela conversa. |

## Onde entra a GenAI

A IA **apoia** o farmacêutico e **não substitui** a orientação dele:

- **Resumo automático da triagem**: um LLM estrutura a dúvida e o histórico informado antes de o profissional entrar na conversa.
- **Checagem de interações**: uma base de dados de medicamentos sinaliza possíveis interações para o farmacêutico revisar.
- **Respostas sugeridas**: rascunhos que o farmacêutico edita e aprova antes de enviar (*human-in-the-loop*).
- **Insights para a farmácia**: dúvidas frequentes por região e categoria, que mostram oportunidades de sortimento e de conteúdo educativo.

## Cuidados regulatórios considerados

- O atendimento é feito por um farmacêutico habilitado e identificado (nome e CRF), conforme as normas do CFF para atenção farmacêutica.
- O chat traz o aviso de que a orientação não substitui uma consulta médica.
- Medicamentos de controle especial exigem a receita na entrega.
- O compartilhamento de dados de saúde depende de consentimento explícito e vale só para aquela conversa (LGPD, art. 11).
- Sinais de emergência direcionam o cliente ao SAMU.

## Métricas para validar

- Taxa de conversão de compra após a conversa, comparada com a de quem não conversou
- Tempo até a primeira resposta do farmacêutico
- Avaliação do atendimento (CSAT)
- Taxa de cancelamento e devolução por compra inadequada

## Próximos passos

- [ ] Painel do farmacêutico: fila de conversas, resumos da IA e alertas de interação
- [ ] Protótipo do resumo da triagem com um LLM
- [ ] Testes de usabilidade com clientes e farmacêuticos

---

**Autora:** Luiza Miller, farmacêutica e mestra em ciências, estudante de Análise e Desenvolvimento de Sistemas
[LinkedIn](https://linkedin.com/in/luiza-miller)
