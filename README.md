O projeto "Get Next Line" tem o objetivo de criar uma função que leia uma linha de um arquivo ou da entrada padrão, uma linha de cada vez, utilizando um descritor de arquivo (fd). A função get_next_line deve retornar a linha lida, incluindo o caractere de nova linha (\n), a não ser que tenha chegado ao final do arquivo. Se não houver mais conteúdo para ler ou se ocorrer um erro, a função deve retornar NULL. O projeto exige que a função seja capaz de lidar com leituras repetidas, garantindo que o comportamento esteja correto tanto para arquivos quanto para a entrada padrão.

A implementação deve utilizar funções como read, malloc e free, além de tratar o fluxo de leitura de maneira eficiente. O uso de variáveis estáticas é necessário para armazenar o estado entre as chamadas da função. A função deve funcionar com um buffer de tamanho configurável, sendo possível definir esse valor durante a compilação com a opção -D BUFFER_SIZE=n. O código precisa ser compilado corretamente tanto com quanto sem o flag -D BUFFER_SIZE. O projeto também exige que o comportamento seja estável, evitando falhas ao ler arquivos binários ou quando o arquivo muda entre chamadas.