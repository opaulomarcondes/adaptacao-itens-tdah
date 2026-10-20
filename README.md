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

## Instalação

A skill é uma pasta com o arquivo `SKILL.md`. A instalação consiste em colocar essa pasta no diretório de skills do assistente.

**Claude Code (terminal ou desktop).** Clone o repositório dentro do diretório de skills pessoais ou do projeto:

```
git clone https://github.com/opaulomarcondes/adaptacao-itens-tdah ~/.claude/skills/adaptacao-itens-tdah
```

Para uso restrito a um projeto, clone em `.claude/skills/adaptacao-itens-tdah/` na raiz dele.

**Claude (aplicativo web ou desktop).** Compacte a pasta `adaptacao-itens-tdah` em um arquivo .zip e envie-o em Configurações, Capacidades, Skills (o caminho exato pode variar conforme a versão do aplicativo).

**Outros assistentes.** O `SKILL.md` é um arquivo Markdown com cabeçalho YAML (`name` e `description`) e pode ser usado como instrução de sistema ou de projeto em qualquer assistente que aceite instruções em texto.

Reinicie a sessão após a instalação para que a skill seja carregada.

## Uso

A skill é acionada quando o pedido envolve adaptar itens, bancos ou provas para estudantes com TDAH. Exemplos de solicitação:

- "Adapte os itens do banco de Ciclos da Vida V para estudantes com TDAH."
- "Gere a versão adaptada das questões 5 a 12 da avaliação, mantendo o gabarito."
- "Este item pode ser adaptado sem alterar o construto?"

Antes de executar, a skill pergunta o escopo: quais itens, como a versão adaptada será entregue, se há política institucional de acomodações e se o número de alternativas permanece em quatro. A entrega é um documento .docx com os itens adaptados e uma tabela de Registro de Adaptações. Um exemplo completo, com item original, item adaptado e registro, está em [`exemplos/exemplo-adaptacao-mcq.md`](exemplos/exemplo-adaptacao-mcq.md).

Entradas esperadas: itens já elaborados, com formato e nível de Bloom definidos no Blueprint. A skill não cria itens novos.

## Estrutura do repositório

| Arquivo | Função |
| --- | --- |
| `SKILL.md` | Instruções da skill: fundamentação, regras, procedimento e checklist |
| `README.md` | Apresentação, instalação e uso |
| `exemplos/exemplo-adaptacao-mcq.md` | Exemplo ilustrativo de adaptação |
| `CITATION.cff` | Metadados para citação |
| `LICENSE` | Texto integral da GNU GPL v3.0 |

## Limites

A skill não diagnostica, não presume TDAH em nenhum estudante e não substitui avaliação multiprofissional nem decisão regulatória. A eficácia das regras para estudantes de medicina não foi testada empiricamente; recomenda-se comparar dificuldade e discriminação dos itens adaptados e originais na análise psicométrica pós-aplicação. A aplicabilidade de normas como a Lei 14.254/2021 ao ensino superior deve ser verificada com assessoria jurídica.

## Origem da ideia

A ideia desta skill surgiu de uma conversa com a profa. Maristela Sanches Bertasso Borges, coordenadora da Central de Apoio e Desenvolvimento do Estudante (CADE/Unirp), a quem registramos o agradecimento.

## Autoria

Paulo Marcondes Carvalho Junior, Instituto Educater (São Paulo), especializado na formação em alto nível na educação médica: desenvolvimento curricular baseado em competências, métodos ativos de ensino-aprendizagem e avaliação de cursos de graduação em medicina.

## Licença

Distribuída sob a licença GNU General Public License v3.0 (GPL-3.0). Obras derivadas que forem distribuídas devem manter a mesma licença e o registro de autoria. O texto integral está em [`LICENSE`](LICENSE).

## Como citar

Carvalho Junior, P. M. *Adaptação de itens de avaliação cognitiva para estudantes com TDAH* (versão 1.0). Instituto Educater, 2026. Disponível em: https://github.com/opaulomarcondes/adaptacao-itens-tdah
