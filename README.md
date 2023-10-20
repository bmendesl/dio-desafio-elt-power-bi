# dio-desafio-elt-power-bi

Descrição do desafio módulo 3 - Processamento de Dados Simplificado com Power BI
1.      Criação de uma instância na Azure para MySQL
2.      Criar o Banco de dados com base disponível no github
3.      Integração do Power BI com MySQL no Azure
4.      Verificar problemas na base a fim de realizar a transformação dos dados
Diretrizes para transformação dos dados
1.      Verifique os cabeçalhos e tipos de dados
        Validados.
2.      Modifique os valores monetários para o tipo double preciso 
        Estão OK, em português decimal fixo.
3.      Verifique a existência dos nulos e analise a remoção 
        Só existe o gerente mas ele possui tem SSNe.
4.      Os employees com nulos em Super_ssn podem ser os gerentes. Verifique se há algum colaborador sem gerente
        Todos estão OK.
5.      Verifique se há algum departamento sem gerente
        Todos Possuem.
6.      Se houver departamento sem gerente, suponha que você possui os dados e preencha as lacunas
        Todos Possuem.
7.      Verifique o número de horas dos projetos
        Validados e adicionados.
8.      Separar colunas complexas
        Separado o endereço.
9.      Mesclar consultas employee e departament para criar uma tabela employee com o nome dos departamentos associados aos colaboradores. A mescla terá como base a tabela employee. Fique atento, essa informação influencia no tipo de junção
10.  Neste processo elimine as colunas desnecessárias
    Realizado
11.  Realize a junção dos colaboradores e respectivos nomes dos gerentes . Isso pode ser feito com consulta SQL ou pela mescla de tabelas com Power BI. Caso utilize SQL, especifique no README a query utilizada no processo.
    Auto relacioanemnto entre employee

 
12.  Mescle as colunas de Nome e Sobrenome para ter apenas uma coluna definindo os nomes dos colaboradores
    Mesclado e criado nome completo
13.  Mescle os nomes de departamentos e localização. Isso fará que cada combinação departamento-local seja único. Isso irá auxiliar na criação do modelo estrela em um módulo futuro.
14.  Explique por que, neste caso supracitado, podemos apenas utilizar o mesclar e não o atribuir.
    Pois o relacionamento é de muitos pra muitos
16.  Agrupe os dados a fim de saber quantos colaboradores existem por gerente
