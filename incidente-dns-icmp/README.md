# Incidente de Segurança Cibernética: Análise de Tráfego DNS e ICMP

Este projeto detalha a investigação de um incidente de rede focado na análise do tráfego DNS e ICMP para identificar o protocolo de rede impactado. A capacidade de analisar dados de ferramentas de monitoramento de rede é fundamental para diagnosticar e responder a eventos de segurança.

**Contexto:** Este trabalho foi desenvolvido como parte do curso de Cibersegurança do Google, simulando um cenário real de análise de incidente para o site `www.yummyrecipesforme.com`.

**Objetivos da Análise:**
*   Analisar o tráfego de rede para identificar a causa da inacessibilidade do site.
*   Determinar o protocolo de rede e o serviço afetados.
*   Documentar as descobertas e as ações recomendadas em um relatório de incidente.

**Habilidades Demonstradas:**
*   Análise de Tráfego de Rede (tcpdump)
*   Diagnóstico de Problemas de Rede (DNS, ICMP, UDP)
*   Identificação de Protocolos e Portas
*   Análise de Incidentes de Segurança
*   Documentação Técnica e Elaboração de Relatórios

**Principais Documentos:**
*   [Cenario_Incidente_Ciberseguranca_DNS_ICMP_yummyrecipesforme.pdf](ciberseguranca-dns-icmp/Cenario_Incidente_Ciberseguranca_DNS_ICMP_yummyrecipesforme.pdf)
*   [Relatóriodeincidentederede_DNS_ICMP_yummyrecipesforme.com.pdf](ciberseguranca-dns-icmp/Relatóriodeincidentederede_DNS_ICMP_yummyrecipesforme.com.pdf)

**Resultados e Descobertas Chave:**
*   O problema principal foi a inacessibilidade da porta UDP 53 (DNS) no servidor `203.0.113.2`, que impedia a resolução do nome de domínio `yummyrecipesforme.com`.
*   As tentativas de resolução DNS resultaram em respostas ICMP com a mensagem "udp port 53 unreachable", indicando que o serviço DNS não estava respondendo ou estava bloqueado.
*   A causa provável do incidente é que o serviço DNS no servidor `203.0.113.2` não estava em execução, estava configurado incorretamente, ou um firewall estava bloqueando o tráfego UDP na porta 53.
