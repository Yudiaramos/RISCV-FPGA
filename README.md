# RISCV-FPGA
Montagem do processador RISC-V (Computação de conjunto de instruções reduzidas) no FPGA, CI totalmente programável, podendo trocar funcionalidades elétricas internas. 

# Por que usar o FPGA?
Usamos o FPGA pela sua principal funcionalidade e vantagem: a flexibilidade do dispositivo, podendo mudar o seu funcionamento simplesmenete fazendo um novo arquivo de configuração.

# O que é o RISC-V?
é um design de microprocessador de código aberto, cujo desenvolvimento é colaborativo e permite que os chips sejam personalizados de acordo com a necessidade de uso por cada organização envolvida na comunidade. 

# Vantagens do RISC-V ISA
Simplicidade, possibilidade do design clean-slate (estaca-zero), extensibilidade e estabilidade.

# RISC-V VS Licensing fees
Criado na Universidade da California, em Berkeley, como trabalho de estudo e pesquisa, RISC-V  vem batalhando contra grandes empresas como a AMD e Intel, que não possuem código aberto para seus chips, dessa forma somente parceiros comerciais têm acesso ao design, como uma alternativa de código aberto e livre de royalties para os concorrentes existentes.

# Projeto:

![CIRCUITO-RISC-V](https://user-images.githubusercontent.com/71808184/208686049-44df5fc7-035b-420f-b45a-f375421ccc62.png)
![placa](https://user-images.githubusercontent.com/71808184/208686066-6ca3918f-cf7a-4511-a50c-7fbaa3adbda3.png)

# 1a etapa --> ULA
bloco que executa operações aritméticas e lógicas. 
Ela soma, subtrai, divide e determina se é positivo, negativo ou zero. Ela pode também executar funções lógicas como “AND”, “OR” ou “OR EXCLUSIVO”.
![ULA](https://user-images.githubusercontent.com/71808184/208688201-12a86de3-ad30-4452-8328-69f9edbf9ee0.png)

# 2a etapa --> Registradores
É um local interno à CPU, onde os dados que foram buscados na memória são armazenados, são usados para armazenar dados da execução do programa, como os valores que serão operados e o resultado das operações. No projeto temos registradores auxiliares (temporários) e de dados (conjunto de instruções).

![registradores](https://user-images.githubusercontent.com/71808184/208688221-b8ff2271-8af9-4612-bca2-2ed015414def.png)

# 3a etapa --> Decodificadores
É um circuito combinatório, que tem o papel de converter um código binário de entrada de N bits em M linhas de saída, de modo que cada linha de saída será ativada por uma única combinação das possíveis de entrada. No projeto foi usado o decodificador Binário para 7 segmentos.

![decodi](https://user-images.githubusercontent.com/71808184/208688240-bcd676a7-249b-4392-95ce-edbfd34a35fd.png)

# 4a etapa --> Contadores
Armarzena numero de vezes que um evento em particular ou processo ocorreu, normalemente em ralação ao sinal de clock.
No projeto, contador binário síncrono (sem atraso) com reset assíncrono (possui atraso de clock).

 ![contador](https://user-images.githubusercontent.com/71808184/208688256-41daeffd-705c-4011-af47-eeedec8188e5.png)
 
## Contribuidores do projeto
# Yudi Asano Ramos - NUSP 1873553 https://github.com/Yudiaramos
# Diogo Barboza de Souza - NUSP 12745657  https://github.com/diogobsouzaa
