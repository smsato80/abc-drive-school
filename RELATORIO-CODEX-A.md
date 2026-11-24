# Relatório — Projeto A

## Implementação

- `index.html` foi reescrito como arquivo único, com CSS e JavaScript embutidos e Google Fonts como única dependência externa. A identidade usa a paleta solicitada, Manrope e Inter; a logo original em base64 foi preservada byte a byte, com largura limitada a 340 px no desktop e a até 240 px no celular.
- Hero atualizado com o texto e os dois destinos solicitados, selo “Projeto demonstrativo” no topo e aviso de escola fictícia no rodapé. As promessas de aprovação e equivalência removidas.
- Simulado com as cinco questões exatas de `questoes-demo.json`, progresso, respostas Certo/Errado, feedback e explicação imediatos, resultado, revisão e opção de refazer. Não usa cadastro, cronômetro nem armazenamento local.
- Abas com recursos descritos para o aluno e protótipo ilustrativo para o instrutor, com dados identificados como fictícios. As referências de formato para Conversão, Karimen e Honmen seguem os números indicados no briefing.
- Metadados de SEO e Open Graph, estados de foco, atributos ARIA, navegação das abas por teclado, transições leves e estilos responsivos adicionados.

## Verificação

- `node --check` no JavaScript extraído: passou.
- Teste automatizado do fluxo JavaScript com DOM simulado: cinco respostas corretas, resultado e revisão, refazer, resposta incorreta e troca de abas passaram.
- Comparação da logo com o arquivo original no Git: conteúdo base64 idêntico (SHA-256 `d0896bad7098bf0d230a6a207156de349bd533ddf11516b029ff177fe39240e7`).
- Comparação dos dados embutidos com `questoes-demo.json`: idênticos. Busca pelas expressões proibidas: nenhuma encontrada.
- O CSS foi inspecionado para layouts de 360 e 390 px, com grades em uma coluna e dimensões flexíveis. Não havia navegador disponível no ambiente para validação visual ou medição de rolagem lateral; esta verificação permanece pendente em navegador real.
- Nenhum commit foi criado.
