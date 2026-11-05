# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users
Professor(a) que corrige pilhas de cartões de resposta de múltipla escolha, no celular, em sala de aula ou em casa. Uso individual, em um único aparelho, sem login. Confirmado pelo usuário.

## Product Purpose
Acelerar a correção de cartões de resposta: ler o cartão pela câmera (modelo Goiás, 40 questões), comparar com o gabarito e registrar acertos por aluno, avaliação e turma. Sucesso é corrigir uma turma inteira com poucos toques e sem digitar respostas.

## Positioning
Leve e privado: roda no navegador do celular, funciona offline, não exige conta e mantém os dados apenas no aparelho. Lê os cartões impressos que a escola já usa.

## Operating Context
- Hierarquia: Turma > Avaliações > Correções (não existe nível de matéria).
- Alunos pertencem à turma, com número de chamada; correções são por avaliação.
- Gabarito oficial definido manualmente ou fotografando um cartão preenchido.
- Marcação '!' = rasura/dupla; vazio = em branco. Só respostas brutas são armazenadas.
- Exportação em CSV e backup/restauração por arquivo.

## Capabilities and Constraints
- HTML/CSS/JS puro, sem build e sem dependências externas; compatível com GitHub Pages.
- Dados somente em localStorage (chave atual `gabarita_v6`); migração segura de versões anteriores, preservando chaves antigas.
- Leitor OMR em JS puro, validado apenas com o modelo Goiás de 40 questões e 7 fotos de teste.
- Interface e terminologia em português do Brasil (turma, avaliação, gabarito, rasura).
- Não testado em celular real nem no Safari.
- Indefinido: gerador de cartões próprios, questão anulada, guia ao vivo na câmera, PWA/offline formal.

## Brand Commitments
Nome: Gabarita. Tom profissional e sóbrio; zero emojis, ícones em SVG.

## Evidence on Hand
Sete fotos de cartões reais em `tests/fixtures/` com gabaritos esperados. Não há depoimentos, clientes ou métricas de uso; não inventar.

## Product Principles
1. Poucos toques por cartão: identificar o aluno, fotografar, conferir.
2. Privacidade por padrão: nada sai do aparelho sem ação explícita do professor.
3. Confiança na leitura: sinalizar dúvida, rasura e alinhamento incerto em vez de adivinhar.
4. Simplicidade sem dependências: preferir solução nativa e dados migráveis sem perda.

## Accessibility & Inclusion
Uso em celular com uma mão; respeitar tema claro/escuro e preferência por reduzir movimento. Nenhum padrão formal adicional foi estabelecido.
