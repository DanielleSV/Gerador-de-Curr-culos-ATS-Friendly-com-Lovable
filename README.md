# 📄 Gerador de Currículos ATS Friendly com Lovable

---

## ✨ Descrição do Projeto
Oi pessoal! 👋  
Quero compartilhar com vocês um projeto que me deixou muito animada: o **Gerador de Currículos ATS Friendly**.  
A ideia surgiu porque muitos currículos bons nunca chegam ao RH — eles são barrados pelos sistemas ATS (Applicant Tracking System) antes mesmo de alguém ler. Então, criei um app que compara o currículo com a descrição da vaga, mostra o nível de compatibilidade, as palavras-chave que estão presentes e aquelas que ainda faltam, e gera uma versão ajustada.  

O mais legal é que o app não inventa nada: ele só reorganiza e sugere melhorias com base na realidade da pessoa candidata. Além disso, tem uma conversa interativa com IA (Vibe Coding), que explica sobre palavras-chave, soft skills e dá dicas éticas de como melhorar a apresentação.  

Ah, e um detalhe importante: o currículo pode ser baixado em **Word (.docx)**, justamente para que o usuário edite livremente antes de enviar.  

🔗 Aplicação publicada: [Meu Currículo com Ética](https://meucurriculocometica.lovable.app/)  
📷 Prints da aplicação: [11 imagens no Canva](https://canva.link/56xy2r2g8r15akx)

---

## 📌 Entendendo o Desafio
O desafio era simples e direto: criar uma aplicação que resolvesse o problema de currículos barrados pelo ATS.  
O núcleo precisava funcionar assim:  
- A pessoa cola a descrição da vaga.  
- A pessoa faz o upload do próprio currículo.  
- O app mostra o match, as palavras-chave encontradas e as que faltam.  
- O app gera a versão ajustada do currículo, pronta para exportar.  

E claro, sempre com a regra principal: **melhorar a apresentação sem inventar experiências ou habilidades**.  

---

## ⚙️ Como Foi Feito
- Escrevi um **mega prompt** em Markdown descrevendo telas, fluxo e design system (shadcn/ui + paleta azul, verde e cinza).  
- Colei esse prompt no Lovable e gerei a primeira versão.  
- Refinei o que veio: pedi ajustes na exportação em PDF e Word, implementei login e autenticação segura, e configurei salvamento de histórico.  
- Publiquei a aplicação com nome, descrição e imagem social.  

---

## 📝 Mega Prompt Utilizado
Gente, esse foi o mega prompt que escrevi para guiar a IA. Ele é grande porque precisava detalhar tudo: telas, fluxo, cores, regras éticas e funcionalidades.  

```markdown
Currículo ATS Friendly
Resumo e relatório do aplicativo — material de estudo

1. Resumo do aplicativo
O Currículo ATS Friendly é um aplicativo web que compara o currículo de uma pessoa candidata com a descrição de uma vaga e gera uma versão ajustada do currículo, otimizada para sistemas de rastreamento de candidatos (ATS). Além da comparação, o app oferece uma conversa interativa com um assistente de inteligência artificial (Vibe Coding), que ensina sobre palavras-chave, soft skills e alinhamento ético do currículo.

2. Telas e fluxo de uso
Tela inicial (painel): upload de currículo e vaga, lista de análises salvas.
Tela de análise: pontuação de compatibilidade, palavras-chave presentes e ausentes, soft skills, gaps, dicas de formatação.
Tela de conversa (Vibe Coding): chat educativo com IA, histórico salvo por análise.
Tela de resultado: currículo ajustado em texto puro, edição livre, exportação em PDF e Word.

3. Regras de ética
- Nunca inventar experiências, formações ou habilidades.
- Lacunas são indicadas como pontos de desenvolvimento.
- Currículo gerado reflete sempre a realidade da pessoa candidata.
- Assistente explica o porquê de cada sugestão.

4. Relatório técnico
Frontend: React 19, TanStack Start, Tailwind CSS v4, shadcn/ui.
Backend: Lovable Cloud com autenticação segura e Row Level Security (RLS).
IA: modelo de linguagem via gateway seguro.
Exportação: jsPDF e docx.
Design: mobile first, fonte Inter, acessibilidade.

5. Conceitos para estudar
ATS, hard skills, soft skills, palavras-chave, Vibe Coding, RLS.
