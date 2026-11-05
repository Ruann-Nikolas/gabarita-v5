# Gabarita v5

Abrir `index.html` no navegador (sem build, sem servidor). Dados ficam no aparelho (localStorage).

Arquivos: `dominio.js` (regras, dados, CSV, backup) · `leitor.js` (leitura do cartão por foto, só modelo Goiás 40 questões) · `app.js` (interface) · `style.css`.

Testes (Node + Playwright): `node --test tests/dominio.test.js`, `node tests/leitor.e2e.js`, `SCRATCH=<pasta> node tests/app.e2e.js`.

Hierarquia: Turma → Avaliações → Correção (alunos pertencem à turma). Dados antigos (v3, v4 e v5, com matéria) são migrados automaticamente; a chave antiga é mantida no navegador.

Limitações: leitura por foto só para o cartão de 40 questões; avaliações com outra quantidade usam correção manual. Testado com 7 fotos (caneta azul e preta).

## Visual (v5)
- Abertura em azul com íris de saída (um toque a encerra); com "reduzir movimento" vira um fade curto.
- Área de trabalho sempre clara (sem modo escuro), responsiva de 320 px a desktop.
- Fonte Inter embutida em `fontes/` (licença em `fontes/LICENCA-Inter.txt`); o app não carrega nada externo.
