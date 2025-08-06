# Análise de Consultas SQL

Este repositório contém um projeto de portfólio focado na aplicação prática de consultas SQL para investigação de segurança em um ambiente corporativo simulado. O objetivo é demonstrar a capacidade de utilizar SQL para analisar dados de tentativas de login e informações de funcionários, identificando atividades suspeitas e contribuindo para a segurança do sistema.

## Cenário

O projeto simula um cenário onde, como profissional de segurança, é necessário investigar possíveis problemas de segurança envolvendo tentativas de login e máquinas de funcionários. As tarefas incluem a recuperação de registros específicos de tabelas `employees` e `log_in_attempts` usando filtros SQL.

## Conceitos SQL Abordados

Este projeto explora a utilização de operadores e cláusulas SQL essenciais para a filtragem e análise de dados:

- **Operadores Lógicos (`AND`, `OR`, `NOT`):** Utilizados para combinar múltiplas condições de filtro, permitindo consultas mais complexas e precisas.
- **Cláusula `LIKE`:** Empregada para buscar padrões específicos em colunas de texto, como identificar tentativas de login de determinados países ou funcionários de escritórios específicos.
- **Filtragem por Data e Hora:** Demonstra como extrair informações baseadas em intervalos de tempo, crucial para investigações de incidentes.

## Consultas e Análises Realizadas

O projeto aborda as seguintes análises, cada uma com sua respectiva consulta SQL e explicação:

1.  **Recuperar tentativas de login com falha após o expediente:** Identificação de logins falhos ocorridos após as 18:00.
2.  **Recuperar tentativas de login em datas específicas:** Análise de tentativas de login em dias específicos (ex: 2022-05-09 e 2022-05-08).
3.  **Recuperar tentativas de login fora do México:** Filtragem de tentativas de login que não se originaram do México.
4.  **Recuperar funcionários em Marketing:** Identificação de funcionários do departamento de Marketing em escritórios específicos (ex: edifício East).
5.  **Recuperar funcionários em Finanças ou Vendas:** Seleção de funcionários dos departamentos de Finanças ou Vendas.
6.  **Recuperar todos os funcionários que não estão na TI:** Exclusão de funcionários do departamento de Tecnologia da Informação.

## Como Visualizar

As capturas de tela das consultas SQL e seus resultados estão incluídas no documento principal do portfólio:

- **[Aplicação de filtros a consultas SQL](https://github.com/samuel-jahnke/meu-portfolio-ciberseguranca/blob/main/analise-de-consultas-SQL/docs/Aplica%C3%A7%C3%A3o%20de%20filtros%20a%20consultas%20SQL.pdf)**
- **[Formato das Tabelas](https://github.com/samuel-jahnke/meu-portfolio-ciberseguranca/blob/main/analise-de-consultas-SQL/docs/Formatos%20das%20Tabelas.pdf)**

Este README serve como um resumo e introdução ao projeto.




