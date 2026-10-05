# 📄 Gerador de Currículos ATS Friendly com Lovable

---

## ✨ Descrição do Projeto
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
- A pessoa faz upload do próprio currículo.  
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
```markdown
# Currículo ATS Friendly
Aplicação web que compara currículo e vaga, mostra compatibilidade, palavras-chave presentes e ausentes, lacunas de soft e hard skills, e gera versão ajustada do currículo.  
Design system: shadcn/ui  
Paleta de cores: azul (#0044cc), verde (#00aa66), cinza claro (#f5f5f5)  
Telas: inicial, análise, conversa (Vibe Coding), resultado.  
Fluxo: upload currículo + vaga → análise → conversa → currículo ajustado → exportação PDF/Word.  
Regras éticas: nunca inventar dados, reforçar aprendizado.  
