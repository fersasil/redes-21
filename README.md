
Como rodar o programa:
gcc router.c -lpthread  -o router && ./router

O router pode ter os seguintes argumentos:

-p ou --port: Número da porta que o router tera
-a ou --address: Endereço ip (ainda não esta funcionando do jeito que deveria)

Caso seja de interesse usar um dos roteadores do arquivo de configuração roteador.config:

--id: Id do roteador do arquivo router.config;

Caso a flag id seja selecionada, as demais serão ignoradas.

O programa não sera iniciado sem ao menos flag port, ou id;

Exemplo de uso:

gcc router.c -lpthread  -o router && ./router -p 8081

gcc router.c -lpthread  -o router && ./router --port 8081


Caso exista um arquivo com o id 1:
gcc router.c -lpthread  -o router && ./router --id 1

Link do github:
https://github.com/fersasil/redes