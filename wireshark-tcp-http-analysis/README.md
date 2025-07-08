# Análise de Tráfego de Rede com Wireshark: Ataque DoS SYN Flood

Este projeto detalha a análise de um incidente de segurança cibernética focado em um ataque de Negação de Serviço (DoS) do tipo SYN Flood, utilizando logs de tráfego de rede capturados com Wireshark. A investigação visa identificar a natureza do ataque, como ele afeta o serviço e as evidências nos logs de rede.

**Contexto:** Este trabalho simula um cenário real onde um servidor web sofre uma interrupção devido a um ataque de inundação SYN, e a análise do tráfego é crucial para entender o incidente.

**Objetivos da Análise:**
*   Identificar o tipo de ataque que causou a interrupção da rede.
*   Explicar o mecanismo do ataque SYN Flood e como ele afeta o servidor web.
*   Analisar os logs de tráfego TCP/HTTP para encontrar evidências do ataque.
*   Documentar as descobertas e as implicações para o serviço.

**Habilidades Demonstradas:**
*   Análise de Tráfego de Rede (Wireshark, tcpdump concepts)
*   Diagnóstico de Ataques de Negação de Serviço (DoS, SYN Flood)
*   Compreensão do Handshake TCP de Três Vias
*   Identificação de Padrões de Tráfego Malicioso
*   Análise de Logs de Segurança
*   Documentação Técnica e Elaboração de Relatórios de Incidente

**Principais Documentos:**
*   [WiresharkTCP_HTTPlog-TCPlog.csv](docs/WiresharkTCP_HTTPlog-TCPlog.csv): Log de tráfego TCP/HTTP capturado.
*   [Relatorio_DoS_SYN_Flood.md](docs/Relatorio_DoS_SYN_Flood.md): Relatório detalhado do incidente, incluindo análise e causas prováveis.

**Resultados e Descobertas Chave:**
*   O incidente foi identificado como um ataque de Negação de Serviço (DoS) por Inundação SYN.
*   Um grande volume de pacotes TCP SYN de um único endereço IP (`203.0.113.0`) sobrecarregou o servidor web (`192.0.2.1`).
*   O servidor esgotou seus recursos ao tentar alocar conexões pendentes, resultando em falha de comunicação para usuários legítimos e mensagens de erro como "HTTP/1.1 504 Gateway Time-out" e pacotes `[RST, ACK]`.
*   A análise dos logs do Wireshark confirmou a inundação de SYNs, as respostas SYN-ACK do servidor sem o ACK final do atacante, e a falha nas conexões legítimas, levando à inacessibilidade total do site.

## Conclusão

Este projeto demonstra a importância da análise de tráfego de rede para identificar e compreender ataques cibernéticos como o SYN Flood. A capacidade de interpretar logs de ferramentas como o Wireshark é fundamental para diagnosticar problemas de segurança e implementar medidas de mitigação eficazes. A interrupção do serviço causada por este ataque ressalta a necessidade de defesas robustas contra ataques de negação de serviço.

