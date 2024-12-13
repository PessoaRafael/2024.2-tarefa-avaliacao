# 2024.2 Avaliação do 1o período de Sistemas Operacionais

## Informações gerais
- **Objetivo do repositório**: Avaliação do 1o bimestre da Disciplina de sistemas operacionais do curso de TADS do IFRN-CNAT
- **Público alvo**: alunos da disciplina de SO (Sistemas Operacionais) do curso de TADS (Superior em Tecnologia em Análise e Desenvolvimento de Sistemas) no CNAT-IFRN (Instituto Federal de Educação, Ciência e Tecnologia do Rio Grande do Norte - Campus Natal-Central).
- disciplina: **SO** Sistemas Operacionais
- professor: [Leonardo A. Minora](https://github.com/leonardo-minora)

## Avaliação
- **Lembre de fazer o fork deste repositório**
- As questões foram construídas com o auxílio do [copilot](https://copilot.microsoft.com/)

# Questão 1. Introdução a sistemas operacionais

Considere as funções e objetivos principais de um sistema operacional conforme discutido no texto. Explique como um sistema operacional gerencia os recursos de hardware e software de um computador para garantir eficiência e segurança. Em sua resposta, aborde os seguintes pontos:

- Gerenciamento de processos
- Gerenciamento de memória
- Gerenciamento de dispositivos de entrada e saída
- Gerenciamento de arquivos

**Dica**: Pense em exemplos práticos de como o sistema operacional realiza essas tarefas no dia a dia de um usuário.

**Copilot informa**: Essa questão incentiva os alunos a explorarem os conceitos fundamentais e a aplicarem o conhecimento teórico em situações práticas. Se precisar de mais alguma coisa, estou aqui para ajudar!

**Resposta**: O sistema operacional (SO) é responsável por gerenciar os recursos de hardware e software de um computador, garantindo eficiência e segurança. O gerenciamento de processos envolve a criação, escalonamento e término de processos, permitindo a execução simultânea de várias tarefas. O SO utiliza algoritmos de escalonamento para otimizar o uso da CPU e isola os processos para evitar interferências, garantindo segurança. No gerenciamento de memória, o SO aloca e libera a memória RAM entre os processos, utilizando técnicas como memória virtual e swap quando a RAM está cheia, evitando falhas no sistema. O gerenciamento de dispositivos de E/S coordena a comunicação entre o sistema e periféricos como teclado, mouse, e impressora, usando drivers para traduzir comandos e assegurar o funcionamento eficiente dos dispositivos sem conflitos. No gerenciamento de arquivos, o SO organiza os dados em sistemas de arquivos, controlando o armazenamento, recuperação e permissões de acesso a arquivos. Ele garante que os dados sejam armazenados de maneira eficiente e segura, com mecanismos de backup e controle de acesso. Em conjunto, esses subsistemas asseguram que o sistema operacional seja capaz de administrar o uso de recursos de forma eficaz, proporcionando ao usuário uma experiência fluida e segura.

# Questão 2. Estrutura de sistemas operacionais

## Texto informativo
### Estrutura de Sistemas Operacionais: Custo de Desenvolvimento e Segurança da Informação

A estrutura de um sistema operacional (SO) é fundamental para determinar tanto o custo de desenvolvimento e manutenção quanto a segurança da informação. Existem várias arquiteturas de SO, como monolítica, microkernel e em camadas, cada uma com suas próprias implicações em termos de custo e segurança.

#### Custo de Desenvolvimento e Manutenção

1. **Arquitetura Monolítica**:
   - **Desenvolvimento**: Geralmente, mais rápida de desenvolver inicialmente, pois todos os componentes do SO são integrados em um único bloco de código.
   - **Manutenção**: Pode ser mais complexa e cara, pois qualquer alteração em um componente pode afetar todo o sistema, exigindo testes extensivos e cuidadosos.

2. **Arquitetura Microkernel**:
   - **Desenvolvimento**: Pode ser mais demorada e cara inicialmente, pois envolve a criação de um núcleo mínimo e a implementação de serviços adicionais como processos separados.
   - **Manutenção**: Mais fácil e menos custosa, já que os componentes são isolados. Atualizações e correções podem ser feitas em módulos específicos sem impactar o núcleo do sistema.

3. **Arquitetura em Camadas**:
   - **Desenvolvimento**: Moderadamente complexa, pois cada camada deve ser bem definida e interagir corretamente com as outras.
   - **Manutenção**: Relativamente fácil, pois problemas podem ser isolados e corrigidos em camadas específicas sem afetar o restante do sistema.

#### Segurança da Informação

1. **Arquitetura Monolítica**:
   - **Segurança**: Pode ser mais vulnerável, pois uma falha em qualquer parte do sistema pode comprometer todo o SO. A integração de todos os componentes em um único bloco de código pode dificultar a implementação de medidas de segurança robustas.

2. **Arquitetura Microkernel**:
   - **Segurança**: Geralmente mais segura, pois isola os serviços em processos separados. Isso limita o impacto de uma falha ou ataque a um único componente, protegendo o núcleo do sistema e outros serviços.

3. **Arquitetura em Camadas**:
   - **Segurança**: Oferece um bom equilíbrio, pois cada camada pode implementar suas próprias medidas de segurança. No entanto, a comunicação entre camadas deve ser cuidadosamente gerenciada para evitar vulnerabilidades.

### Conclusão

A escolha da arquitetura de um sistema operacional tem um impacto significativo tanto no custo de desenvolvimento e manutenção quanto na segurança da informação. Arquiteturas monolíticas podem ser mais rápidas e baratas de desenvolver inicialmente, mas podem acarretar custos de manutenção mais altos e maiores riscos de segurança. Por outro lado, arquiteturas microkernel e em camadas podem exigir um investimento inicial maior, mas oferecem vantagens em termos de manutenção e segurança.

## Questão
Com base no texto sobre a estrutura de sistemas operacionais, analise como as diferentes arquiteturas (monolítica, microkernel e camadas) impactam o custo com a equipe de desenvolvimento e a segurança do sistema operacional. Em sua resposta, considere os seguintes pontos:
- Complexidade de implementação e manutenção
- Necessidade de especialização da equipe
- Potenciais vulnerabilidades de segurança
- Facilidade de atualização e correção de falhas

**Dica:** Utilize exemplos de sistemas operacionais reais que adotam essas arquiteturas para ilustrar sua análise.

**Copilot informa**: Essa questão incentiva os alunos a considerarem tanto os aspectos econômicos quanto os de segurança ao avaliar diferentes arquiteturas de sistemas operacionais.

**Resposta**: A arquitetura de um sistema operacional (SO) influencia diretamente o custo de desenvolvimento, a manutenção e a segurança. Na arquitetura monolítica, todos os componentes estão integrados em um único código, o que facilita o desenvolvimento inicial, mas torna a manutenção mais cara e complexa, além de aumentar as vulnerabilidades de segurança, já que uma falha em um módulo pode comprometer todo o sistema. Exemplos incluem o Linux e versões antigas do Unix. Já na arquitetura microkernel, o núcleo é mínimo, com serviços isolados em módulos, o que aumenta a segurança e facilita a manutenção, embora o desenvolvimento inicial seja mais demorado e custoso. Sistemas como o MINIX e QNX seguem esse modelo, sendo usados em sistemas críticos. Por fim, a arquitetura em camadas divide o sistema em camadas independentes, facilitando a manutenção e a atualização, pois falhas podem ser isoladas em camadas específicas. Exemplo disso são os sistemas Windows NT e OS/2. Cada arquitetura oferece vantagens e desvantagens em termos de custo, segurança e facilidade de manutenção, sendo a escolha dependente das necessidades específicas do projeto.

# Questão 3. Introdução à Segurança de Sistemas Operacionais

## Texto informativo

A segurança de um sistema operacional é um aspecto crucial que visa proteger os recursos do sistema contra acessos não autorizados, ataques maliciosos e falhas. Um sistema operacional seguro deve garantir a integridade, confidencialidade e disponibilidade dos dados e serviços. Para alcançar esses objetivos, várias técnicas e mecanismos são implementados, incluindo:

1. **Controle de Acesso**: Define quem pode acessar o sistema e quais recursos podem ser utilizados. Isso é feito através de autenticação (verificação de identidade) e autorização (permissão de acesso).

2. **Criptografia**: Utilizada para proteger dados em trânsito e em repouso, garantindo que apenas usuários autorizados possam acessar informações sensíveis.

3. **Auditoria e Monitoramento**: Registra atividades do sistema para detectar e responder a comportamentos suspeitos ou anômalos.

4. **Isolamento de Processos**: Garante que os processos sejam executados em ambientes isolados, evitando que um processo comprometa a segurança de outro.

5. **Atualizações e Patches**: Manter o sistema operacional atualizado é essencial para corrigir vulnerabilidades conhecidas e proteger contra novas ameaças.


## Questão

Considerando os mecanismos de segurança discutidos, analise como a implementação de controles de acesso e criptografia pode impactar a performance e a usabilidade de um sistema operacional. Em sua resposta, aborde os seguintes pontos:
- Benefícios e desafios de cada mecanismo
- Impacto na experiência do usuário
- Exemplos de situações onde esses mecanismos são críticos

**Dica:** Pense em como esses mecanismos são aplicados em sistemas operacionais que você utiliza no dia a dia, como Windows, Linux ou macOS.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre o equilíbrio entre segurança, performance e usabilidade, aplicando conceitos teóricos a contextos práticos.

**Resposta**: A implementação de controles de acesso e criptografia em sistemas operacionais traz grandes benefícios para a segurança, mas também desafios em termos de performance e usabilidade. Os controles de acesso protegem contra acessos não autorizados, garantindo a integridade e confidencialidade dos dados, mas podem afetar a performance, especialmente em processos de autenticação, como a multifatorial. A experiência do usuário também pode ser impactada, com procedimentos de login mais demorados e restrições no uso dos recursos. Sistemas como Windows e Linux aplicam permissões para gerenciar o acesso a arquivos e serviços, sendo essenciais em ambientes com dados sensíveis. Já a criptografia, que protege dados em trânsito e em repouso, garante a segurança das informações, mas pode diminuir a performance, especialmente em dispositivos mais lentos, ao exigir processamento adicional para criptografar e descriptografar dados. Isso pode afetar a velocidade de acesso e a experiência do usuário, como em dispositivos móveis. No entanto, em contextos críticos, como e-commerce e armazenamento de dados confidenciais, ambos os mecanismos são fundamentais, e o desafio está em equilibrar segurança com eficiência.

# Questão 4. Custo de Processamento versus Algoritmo Ótimo de Escalonamento

## Texto informativo

O escalonamento de processos é uma função crítica de um sistema operacional, responsável por determinar a ordem em que os processos são executados pelo processador. O objetivo é maximizar a eficiência do sistema, garantindo que os recursos sejam utilizados de maneira justa e eficaz. No entanto, encontrar o algoritmo de escalonamento ótimo envolve um equilíbrio delicado entre o custo de processamento e a eficiência do escalonamento.

### Custo de Processamento

O custo de processamento refere-se ao tempo e aos recursos necessários para executar um algoritmo de escalonamento. Algoritmos mais complexos podem oferecer melhores resultados em termos de tempo de resposta e utilização do processador, mas também podem exigir mais recursos computacionais para tomar decisões de escalonamento. Isso pode incluir tempo de CPU, memória e outras operações de sistema.

### Algoritmo Ótimo de Escalonamento

Um algoritmo ótimo de escalonamento é aquele que maximiza a eficiência do sistema operacional, minimizando o tempo de espera dos processos, o tempo de resposta e o tempo de retorno. Alguns dos algoritmos de escalonamento mais comuns incluem:

- **First-Come, First-Served (FCFS)**: Simples e fácil de implementar, mas pode levar a longos tempos de espera para processos curtos.
- **Shortest Job Next (SJN)**: Minimiza o tempo médio de espera, mas pode ser difícil de implementar devido à necessidade de prever o tempo de execução dos processos.
- **Round Robin (RR)**: Oferece uma abordagem justa, atribuindo fatias de tempo iguais a todos os processos, mas pode resultar em maior sobrecarga de contexto.
- **Priority Scheduling**: Processos com maior prioridade são executados primeiro, mas pode levar à inanição de processos de baixa prioridade.

## Questão

Considerando os conceitos de custo de processamento e algoritmo ótimo de escalonamento, analise como diferentes algoritmos de escalonamento podem impactar a performance de um sistema operacional em termos de tempo de resposta, tempo de espera e utilização do processador. Em sua resposta, aborde os seguintes pontos:
- Vantagens e desvantagens de pelo menos dois algoritmos de escalonamento
- Impacto do custo de processamento na escolha do algoritmo
- Exemplos de situações onde um algoritmo pode ser preferível a outro

**Dica:** Pense em como esses algoritmos são aplicados em diferentes cenários, como sistemas de tempo real, servidores web e sistemas operacionais de uso geral.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre a complexidade e os trade-offs envolvidos na escolha de um algoritmo de escalonamento, aplicando conceitos teóricos a contextos práticos.

**Resposta**: Os algoritmos de escalonamento de processos impactam diretamente o tempo de resposta, tempo de espera e a utilização do processador de um sistema operacional. O First-Come, First-Served (FCFS) é simples e fácil de implementar, mas pode resultar em longos tempos de espera para processos curtos, o que compromete a eficiência do sistema, especialmente em cenários com processos de durações variadas. Por outro lado, o Round Robin (RR) é mais justo, garantindo que todos os processos recebam uma fatia de tempo igual, o que melhora o tempo de resposta em sistemas interativos. No entanto, o RR pode causar sobrecarga de contexto, reduzindo a utilização do processador devido ao tempo gasto trocando entre processos. O custo de processamento dos algoritmos também é um fator crucial, pois algoritmos mais complexos, como o Shortest Job Next (SJN), exigem mais recursos computacionais para prever o tempo de execução dos processos, mas podem ser mais eficientes em termos de tempo de espera. A escolha do algoritmo depende do tipo de sistema: em sistemas de tempo real, algoritmos como SJN ou Prioridade são ideais para minimizar o tempo de resposta de processos críticos, enquanto em servidores web, o Round Robin é eficaz para distribuir recursos de forma justa entre múltiplos usuários. Em sistemas de uso geral, combinações de algoritmos, como Round Robin e Prioridade, podem equilibrar a equidade e a eficiência. A escolha do algoritmo de escalonamento deve considerar o desempenho e a natureza dos processos envolvidos.

# Questão 5. Aplicativo em python vs aplicativos em c

## Questão

Explique o caminho que as instruções seguem desde um aplicativo escrito em Python e um aplicativo escrito em linguagem C até serem executadas pelo hardware. Em sua resposta, considere os seguintes pontos:
- O papel do interpretador no caso do Python
- O processo de compilação no caso do C
- A interação entre o kernel do sistema operacional e os drivers de dispositivo
- A tradução final das instruções para o formato binário (0 e 1) executado pelo hardware

**Dica:** Compare e contraste os dois processos, destacando as principais diferenças e semelhanças na forma como as instruções são processadas e executadas.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre os diferentes caminhos que as instruções seguem em linguagens interpretadas e compiladas, aplicando conceitos teóricos a contextos práticos.

**Resposta**: A execução de aplicativos escritos em **Python** e **C** segue caminhos distintos, principalmente devido à diferença entre **linguagens interpretadas** e **compiladas**. No caso do Python, que é interpretado, o código-fonte é traduzido em **bytecode** pelo interpretador, como a **máquina virtual Python (PVM)**. O bytecode é então executado em tempo real, sendo convertido em instruções de baixo nível durante a execução. O interpretador gerencia a comunicação com o **kernel do sistema operacional**, que aloca recursos e interage com os **drivers de dispositivos**, como memória e dispositivos de entrada/saída. O Python, portanto, não gera diretamente código binário de máquina; ele executa as instruções dinamicamente enquanto o programa roda. Em contraste, no **C**, que é compilado, o código-fonte passa por várias etapas: o **pré-processamento**, a **compilação** para código objeto e, por fim, o **linkedição** para gerar um arquivo executável. Esse arquivo contém **código binário** que o processador pode executar diretamente, sem a necessidade de um interpretador. O kernel, após carregar o executável, aloca recursos e interage com os drivers de dispositivo, enquanto o código binário é executado pelo processador. A principal diferença entre os dois métodos é que o Python, por ser interpretado, tem desempenho inferior devido ao overhead de tradução em tempo real, enquanto o C, por ser compilado, oferece maior desempenho, pois é convertido diretamente em código de máquina. Python é mais portável, pois depende do interpretador, enquanto C precisa ser recompilado para cada plataforma. Ambos os métodos interagem com o kernel para gerenciar os recursos do sistema, mas a forma como as instruções são traduzidas e executadas no hardware varia, com o Python utilizando um interpretador e o C utilizando código binário compilado.
