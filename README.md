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
## 📝 Mega Prompt Utilizado

Este foi o mega prompt que escrevi para guiar a IA na criação do app. Ele é detalhado porque precisava descrever telas, fluxo, cores, regras éticas e funcionalidades:

```markdown
# Currículo ATS Friendly com Lovable

Aplicação web que compara currículo e vaga e gera uma versão ATS friendly.  

## Design
- Design system: shadcn/ui  
- Paleta de cores: azul (#0044cc), verde (#00aa66), cinza claro (#f5f5f5)  
- Fonte: Inter  
- Layout: mobile first, acessibilidade garantida  

## Telas
- **Tela inicial (painel)**: upload de currículo e vaga, lista de análises salvas  
- **Tela de análise**: pontuação de compatibilidade (0 a 100), palavras-chave presentes e ausentes, soft skills, gaps, dicas de formatação  
- **Tela de conversa (Vibe Coding)**: chat educativo com IA, histórico salvo por análise  
- **Tela de resultado**: currículo ajustado em texto puro, edição livre, exportação em PDF e Word  

## Fluxo
Upload currículo + vaga → análise → conversa → currículo ajustado → exportação PDF/Word  

## Regras éticas
- Nunca inventar experiências, formações ou habilidades  
- Lacunas são indicadas como pontos de desenvolvimento  
- Currículo gerado reflete sempre a realidade da pessoa candidata  
- Assistente explica o porquê de cada sugestão  

## Tecnologias
- **Frontend**: React 19, TanStack Start, Tailwind CSS v4, shadcn/ui  
- **Backend**: Lovable Cloud com autenticação segura e Row Level Security (RLS)  
- **IA**: modelo de linguagem via gateway seguro  
- **Exportação**: jsPDF e docx  
- **Infra**: publicação no Lovable Cloud  


---

## 🚧 Gargalos e Aprendizados
Durante o desenvolvimento, encontrei algumas dificuldades que vale destacar:  
- Como estou estudando, usei a versão **gratuita do Lovable**, o que limitou os créditos e fez com que o desenvolvimento levasse **três dias** para ser concluído. Esse foi um dos gargalos principais.  
- Outro gargalo foi a área de **Vibe Coding**, que ainda precisa de ajustes para ficar mais fluida e completa. Mesmo assim, decidi publicar a aplicação dentro do prazo do curso para mostrar o resultado final.  
- A exportação em Word foi um ponto que precisei ajustar, mas acabou sendo um diferencial importante para permitir edição livre do currículo.  
- Para evidenciar o funcionamento, subi **11 prints do app** neste link: [Canva com prints](https://canva.link/56xy2r2g8r15akx).  
- Aprendi que clareza nos prompts e foco no essencial ajudam a economizar tempo e créditos, além de garantir que a aplicação seja funcional mesmo em versão gratuita.  

---

## 🚀 Ideias para Evoluir
- Melhorar a área de Vibe Coding para deixar a experiência mais fluida.  
- Exportar currículo também em outros formatos além de PDF e Word.  
- Guardar histórico das análises em banco de dados.  
- Criar login com confirmação por e-mail para segunraça.  
- Montar dashboard mostrando evolução do match.  
- Especializar saída em nichos (tecnologia, primeiro emprego).  
- Preparar aplicação para SEO e GEO (buscas dentro das IAs).  

---

## 🎯 Reflexões
- O que funcionou bem: clareza nos prompts (que estou aprendendo com a DIO) e implementação das regras éticas.  
- O que não funcionou: limite de créditos e ajustes incompletos no Vibe Coding.  
- O que aprendi: importância da clareza e intenção ao conversar com IA, valor do Vibe Coding e da ética no desenvolvimento de soluções.  
- Documentar gargalos e soluções fortaleceu o projeto pra mim.  
