# Adaptação de itens de avaliação cognitiva para estudantes com TDAH

Skill para assistentes de IA (formato `SKILL.md`) que adapta itens de avaliação cognitiva já elaborados para estudantes de medicina com diagnóstico de Transtorno do Déficit de Atenção/Hiperatividade (TDAH), reduzindo a carga cognitiva extrínseca sem alterar construto, nível da Taxonomia de Bloom, dificuldade ou gabarito.

## Princípio

A adaptação é uma acomodação, não uma simplificação. Remove-se o que não pertence ao construto avaliado (extensão desnecessária, sintaxe encadeada, negações, dados dispersos, alternativas combinatórias, distratores que diferem por detalhe mínimo). Preserva-se tudo o que sustenta o raciocínio exigido pelo objetivo de aprendizagem.

## Conteúdo

O arquivo [`SKILL.md`](SKILL.md) reúne:

- uma síntese das características do TDAH relevantes para a avaliação, com marcação de confiança em cada afirmação e ressalvas sobre a heterogeneidade do transtorno e a evidência limitada sobre adaptações de itens;
- 36 regras de adaptação, organizadas em oito blocos: invariantes de validade, carga de leitura e estrutura do enunciado, memória operacional, alternativas (mcq), atenção sustentada e inibição, formatos MEQ, essay e dissertativa, apresentação gráfica e acomodações administrativas;
- procedimento de execução, checklist de equivalência e formato de saída (.docx com tabela de registro de adaptações);
- limites de uso e referências.

## Formatos de item contemplados

| Formato | Descrição |
| --- | --- |
| mcq | Múltipla escolha tipo A, quatro alternativas (A a D), padrão NBME |
| MEQ | Interrogativa única, resposta curta em prosa, sem rubrica |
| essay | Interrogativa única, resposta em prosa de até três linhas |
| dissertativa | Comando estruturado com subitens ponderados e rubrica analítica |

Formato e nível de Bloom são entradas independentes, definidas no Blueprint, e nunca são alterados pela skill.

## Como usar

Copie a pasta para o diretório de skills do seu assistente (por exemplo, `.claude/skills/adaptacao-itens-tdah/`) e solicite, por exemplo: "Adapte os itens do banco de Ciclos da Vida V para estudantes com TDAH". A skill pergunta o escopo (itens, forma de entrega, política institucional de acomodações, número de alternativas) antes de executar.

## Limites

A skill não diagnostica, não presume TDAH em nenhum estudante e não substitui avaliação multiprofissional nem decisão regulatória. A eficácia das regras para estudantes de medicina não foi testada empiricamente; recomenda-se comparar dificuldade e discriminação dos itens adaptados e originais na análise psicométrica pós-aplicação. A aplicabilidade de normas como a Lei 14.254/2021 ao ensino superior deve ser verificada com assessoria jurídica.

## Autoria

Paulo Marcondes Carvalho Junior, [Instituto Educater](https://github.com/opaulomarcondes) (São Paulo), consultoria especializada em educação médica: desenvolvimento curricular baseado em competências, métodos ativos de ensino-aprendizagem e avaliação de cursos de graduação em medicina.
