Permissões de Arquivo no Linux

Este projeto demonstra a aplicação prática do controle de acesso no Linux, focando na auditoria e modificação de permissões de arquivos e diretórios. O objetivo foi garantir a segurança e a integridade dos dados em um ambiente simulado de equipe de pesquisa, alinhando as permissões com as políticas de segurança.

Descrição do Projeto

Como parte de uma iniciativa de segurança para uma equipe de pesquisa, foi necessário auditar e atualizar as permissões de arquivos e diretórios no diretório projects. As permissões existentes não refletiam o nível de autorização adequado, representando um risco de segurança. Para mitigar esse risco, realizei uma análise e reconfiguração das permissões para garantir que apenas usuários autorizados tivessem o acesso apropriado, fortalecendo a segurança do sistema.

Tecnologias Utilizadas

•
Linux: Sistema operacional base para a execução dos comandos.

•
Comandos de Terminal:

•
ls -la: Para listar arquivos e diretórios com detalhes de permissão.

•
chmod: Para modificar as permissões de arquivos e diretórios.



Como Executar

Para replicar este projeto, siga os passos abaixo em um ambiente Linux:

1.
Acessar o diretório de projetos:

2.
Verificar as permissões atuais:

3.
Remover permissão de escrita para 'outros' em project_k.txt:

4.
Definir permissão de leitura para usuário e grupo em .project_x.txt:

5.
Remover permissão de execução para o grupo em drafts:

Contribuição

Sinta-se à vontade para explorar, sugerir melhorias ou adaptar este projeto para seus próprios estudos e portfólio de cibersegurança.


