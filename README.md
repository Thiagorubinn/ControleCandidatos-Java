# ControleCandidatos-Java

## Documentação do Código - Processo Seletivo

Este é um programa Java que simula um processo seletivo para uma vaga de emprego, onde candidatos são contatados, avaliados com base em seus salários pretendidos e selecionados se suas expectativas salariais forem atendidas. O programa utiliza métodos para modularizar suas funcionalidades e realiza interações com os candidatos e suas informações.

### Funcionalidades Principais

1. **Entrando em Contato com Candidatos**

   O método `entrandoEmContato(String candidato)` tenta entrar em contato com um candidato, realizando até 3 tentativas. A cada tentativa, o método verifica se o candidato atendeu o telefone. Se o candidato atender, exibe uma mensagem de sucesso, caso contrário, continua tentando. O resultado de todas as tentativas é apresentado ao final.

2. **Método de Atendimento**

   O método `atender()` gera um resultado aleatório (1/3 de chance de ser verdadeiro), simbolizando se o candidato atendeu ao telefone.

3. **Impressão de Candidatos Selecionados**

   O método `imprimirSelecionados()` imprime uma lista de candidatos selecionados, mostrando o índice do elemento e o nome do candidato. Duas abordagens são usadas para a iteração: uma usando o índice tradicional e outra utilizando o loop "for-each".

4. **Seleção de Candidatos**

   O método `selecaoCandidatos()` simula o processo de seleção de candidatos com base em seus salários pretendidos. Ele itera pelos candidatos, verifica seus salários pretendidos e seleciona até 5 candidatos cujas expectativas salariais sejam atendidas.

5. **Geração de Salário Pretendido**

   O método `valorPretendido()` gera um valor aleatório entre 1800 e 2200 para representar o salário pretendido por um candidato.

6. **Análise de Candidato**

   O método `analisarCandidato(double salarioPretendido)` compara o salário base (2000.0) com o salário pretendido do candidato. Com base nessa comparação, decide se deve ligar para o candidato, propor uma contra proposta ou aguardar resultados de outros candidatos.

### Utilização

1. **Main Method (ProcessoSeletivo.main())**

   A função principal do programa inicia o processo seletivo ao entrar em contato com cada candidato usando o método `entrandoEmContato()`. Para cada candidato, o programa tenta contatá-lo e exibe o resultado das tentativas.

2. **Método de Entrar em Contato (entrandoEmContato(String candidato))**

   Este método gerencia as tentativas de contato com um candidato específico, imprimindo mensagens conforme o contato seja bem-sucedido ou não.

3. **Método de Atendimento (atender())**

   Gera um resultado aleatório (1/3 de chance) para simular se o candidato atendeu ao telefone.

4. **Impressão de Candidatos Selecionados (imprimirSelecionados())**

   Este método itera sobre a lista de candidatos e imprime seus nomes e índices, utilizando tanto o índice tradicional quanto o loop "for-each".

5. **Seleção de Candidatos (selecaoCandidatos())**

   Simula a seleção de candidatos com base em seus salários pretendidos, imprimindo informações sobre o processo de seleção.

6. **Geração de Salário Pretendido (valorPretendido())**

   Gera um valor aleatório entre 1800 e 2200 para representar o salário pretendido por um candidato.

7. **Análise de Candidato (analisarCandidato(double salarioPretendido))**

   Compara o salário base com o salário pretendido do candidato e decide como proceder com base nessa comparação.

### Considerações Finais

Este programa Java demonstra um processo seletivo fictício, mostrando como entrar em contato com candidatos, avaliar suas expectativas salariais e selecionar os melhores candidatos. Os métodos modulares tornam o código mais legível e facilitam a manutenção e expansão do programa. É importante notar que esse código pode ser expandido e aprimorado para incluir mais recursos, como armazenamento persistente de informações de candidatos, análise de currículos e assim por diante.
