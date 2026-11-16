# Catálogo de produtos com paginação

**Status: planejamento — implementação ainda não iniciada.**

Repositório de estudo de [José Carlos](https://github.com/carlos0ff), organizado a partir da [seleção de desafios de Matheus Leandro](https://www.matheusleandro.com.br/desafios).

## Objetivo

Desenvolver um catálogo que consulte produtos em páginas e permita navegar pelos resultados sem recarregar toda a interface.

## Escopo do desafio

- Persistir `Product` com JPA e acesso via `JpaRepository`.
- Disponibilizar a listagem em `/api/v1/product`.
- Limitar cada página a 100 registros.
- Encapsular resultados e metadados em `PageResponse<T>`.
- Criar uma interface em HTML e JavaScript com navegação anterior/próxima.
- Utilizar PostgreSQL, com banco `produtos`.

## Atenção ao contrato

O enunciado pede um DTO com `name` e `price`, mas também solicita `createdAt` na interface. A solução deverá registrar como esse campo será disponibilizado e manter backend e frontend consistentes.

## Critérios de conclusão

- [ ] Implementar persistência e paginação.
- [ ] Definir parâmetros e formato da resposta.
- [ ] Testar páginas vazias, primeira/última página e limite máximo.
- [ ] Integrar a interface e tratar falhas de consulta.
- [ ] Documentar configuração do banco e comandos de execução.

## Tecnologias previstas

Java, Spring Boot, Spring Data JPA, PostgreSQL, HTML e JavaScript. Versões e ferramenta de build ainda serão definidas; credenciais deverão vir da configuração local.

## Como executar

Este repositório contém apenas a documentação inicial. Ainda não há aplicação, scripts de execução ou testes executáveis. Os comandos serão adicionados junto com a implementação.

## Referências e créditos

- [Enunciado na plataforma](https://www.matheusleandro.com.br/desafios/desafio-full-stack-com-paginacao)
- [Referência original indicada pela plataforma](https://github.com/matheuslf/dev-matheuslf-desafio-fullstack)

Este README resume a proposta e registra um plano de trabalho. Os créditos do enunciado pertencem aos autores das referências; a solução será desenvolvida neste repositório.
