# Projeto A — ABC Drive School v2 (executor: Codex; coordenação/auditoria: Muse)

Reescrever `index.html` desta pasta (arquivo único, sem dependências além do Google Fonts já usado) aplicando:

## Identidade (preservar)
Paleta do kit ABC: #0B0D10, #1A1E24, #22272F, #B89A5A, #D6BC7E, #D9DDE3, #F5F3EE, cinzas #8D949D/#C9CDD3. Fontes Manrope (títulos) e Inter (texto). A logo embutida em base64 no arquivo atual deve ser MANTIDA byte a byte (não trocar a imagem), só que MENOR: no celular, largura máxima ~240px; no desktop ~340px.

## Mensagem (substituir a atual)
- Título: "Prepare-se para conquistar sua habilitação no Japão."
- Subtítulo: "Estude as regras de trânsito em português, pratique com simulados online e acompanhe sua evolução até o dia da prova."
- CTAs: "Experimentar simulado" (rola até a demonstração) e "Conhecer a plataforma" (rola até as abas).
- PROIBIDO: "sem reprovar", "aprovação garantida", "questões idênticas à prova oficial" ou qualquer promessa de aprovação. A frase atual do hero contém "sem reprovar" e deve sair.
- Selo elegante e visível no topo: "Projeto demonstrativo" (discreto, premium, sem quebrar o design). Rodapé mantém o aviso de escola fictícia.

## Simulado demonstrativo funcional (novo, no lugar do cartão estático)
Usar as 5 questões de `questoes-demo.json` (nesta pasta), embutidas no JS da página:
- Uma questão por vez, botões Certo/Errado, barra de progresso (Questão X de 5).
- Ao responder: feedback imediato (acertou/errou), explicação da questão, botão "Próxima".
- No fim: resultado (X de 5), revisão curta das respostas e botão "Refazer".
- Sem cadastro, sem cronômetro, sem localStorage.
- Rótulo junto ao simulado: "Demonstração com 5 questões de estudo. Material independente, não é a prova oficial."
- Formatos oficiais corretos quando citados: Conversão = 50 questões, 30 min, aprovação com 45 acertos (90%). Karimen = 50 questões, 30 min, 45+. Honmen = 100 pontos (90 de texto + ilustração), 50 min, 90+.

## Abas "Visão do aluno" / "Visão do instrutor"
- Aluno: o que existe de verdade na plataforma completa (simulados com cronômetro, revisão com explicações, histórico e melhor nota salvos no aparelho).
- Instrutor: PROTÓTIPO claramente rotulado "Protótipo ilustrativo": cartão de exemplo com dados 100% fictícios marcados como fictícios (ex.: "Aluno A — exemplo fictício"), mostrando acompanhamento de notas e dificuldades. Nunca afirmar que está entregue/operacional.

## Qualidade
Responsivo (360/390px sem rolagem lateral), microinterações leves (transições de hover/foco), acessibilidade básica (foco visível, aria nas abas e no quiz), SEO (title/description/og), JS sem erros (node --check no script extraído). Registrar tudo em RELATORIO-CODEX-A.md. NÃO fazer commit. Não tocar em outros arquivos além de index.html, questoes-demo.json (leitura) e o relatório.
