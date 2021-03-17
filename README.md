# Template Github Professional

Este repositório é uma ferramenta poderosa para desenvolver a capacidade dos alunos em organizar os seus estudos,
os códigos fontes, a documentação e tudo que é útil para um programador profissional ser produtivo.


## Índice

- [Objetivo](#objetivo)
- [Cursos e Github](#cursos-e-github)
- [Como usar este template](#como-usar-este-template)
- [Clonando o repositório e trabalhando na sua IDE](#Clonando-o-repositório-e-trabalhando-na-sua-IDE)
- [Conclusão](#conclusão)

## Objetivo

Concluir os Cursos colocando em prática o uso do Github

## Cursos e Github

Aqui estão as definições dos recursos de cada plataforma e como eles se relacionam.

| Cursos | <-> | Github |
| :---: | :---: | :---:|
| Curso | <-> | Milestones |
| Tópicos | <-> | Issues |
| Grupo de Aulas | <-> | Branchs
| Nível | <-> | Labels

- Cada `Curso` é um `Milestone`
- Cada `Tópico do curso` é um `Issue`
- Cada `Grupo de aula` é um `Branch`
- Cada `Nível` é um `Label`

## Como usar este template

1. Faça um _Fork_ deste repositório, configure-o com as opções abaixo:
    * Em **Settings > Options**, marque estas opções:
        - `Features`
            - [x] Issues
        - `Merge Button`
            - [x] Allow auto-merge
            - [x] Automatically delete head branches
    * Em **Issues > Milestones**, crie um milestone com o prefixo `Curso - ` e o nome do Curso
      e o prazo de finalização.
      Ex:
      >Curso - Gostack
    * Em **Issues > Labels**, apague todas e crie estas 3:  
      `basic` `intermediary` `advanced`

1. Para cada tópico do curso, crie um `issue` e relacione `label` e `milestone`

## Clonando o repositório e trabalhando na sua IDE

1. Clone este repo:
   `git clone https://github.com/<USERNAME>/template-github-professional.git`

1. Para cada grupo de aula, crie um `branch` com o nome do grupo de aula e faça seus `commits` e `pushs`
1. Após concluir um curso, faça um `pull request (PR)` e relacione com o `issue` do topico de curso

## Conclusão

O status do seu curso (milestone) será atualizado a cada vez que você concluir um tópico de curso.
E sua missão é completar todos os tópicos para completar os seus estudos.


- Seu `PR` será fechado automaticamente (merge automático)
- Seu `branch` será integrado ao `main` e então excluído
- Seu `issue` é fechado por conta da conclusão do `PR` linkado à ele
- Seu `milestone` é atualizado com o status desse `issue` concluído

> `Dica` Documente sua evolução, preencha o README de cada aula com o que fez mais sentido pra você

![parabéns](https://media.giphy.com/media/xT0xezQGU5xCDJuCPe/giphy.gif)
