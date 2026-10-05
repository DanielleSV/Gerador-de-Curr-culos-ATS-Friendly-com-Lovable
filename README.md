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
- A pessoa cola o próprio currículo.  
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
# Currículo ATS Friendly com Lovable

Aplicação web que compara currículo e vaga e gera uma versão ATS friendly.  

Design system: shadcn/ui  
Paleta de cores: azul (#0044cc), verde (#00aa66), cinza claro (#f5f5f5)  

### Telas
- **Tela inicial (painel)**: upload de currículo e vaga, lista de análises salvas.  
- **Tela de análise**: pontuação de compatibilidade (0 a 100), palavras-chave presentes e ausentes, soft skills, gaps, dicas de formatação.  
- **Tela de conversa (Vibe Coding)**: chat educativo com IA, histórico salvo por análise.  
- **Tela de resultado**: currículo ajustado em texto puro, edição livre, exportação em PDF e Word.  

### Fluxo
Upload currículo + vaga → análise → conversa → currículo ajustado → exportação PDF/Word.  

### Regras éticas
- Nunca inventar experiências, formações ou habilidades.  
- Lacunas são indicadas como pontos de desenvolvimento.  
- Currículo gerado reflete sempre a realidade da pessoa candidata.  
- Assistente explica o porquê de cada sugestão.  

### Tecnologias
- **Frontend**: React 19, TanStack Start, Tailwind CSS v4, shadcn/ui  
- **Backend**: Lovable Cloud com autenticação segura e Row Level Security (RLS)  
- **IA**: modelo de linguagem via gateway seguro  
- **Exportação**: jsPDF e docx  
- **Design**: mobile first, fonte Inter, acessibilidade  
