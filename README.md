# EstudosIA
**Aula 02 - Introdução à Inteligência Artificial** 

### 1. **O que é Inteligência Artificial (IA)?**
- IA busca **compreender e construir** entidades inteligentes que possam realizar tarefas que exigem **pensamento humano**, como tomar decisões, resolver problemas e aprender.

### 2. **Pontos de Vista sobre IA**
- **Pensando como humanos**: IA tenta replicar o pensamento humano e resolver problemas da mesma forma que as pessoas.
- **Agindo como humanos**: Exemplo clássico é o **Teste de Turing**, que verifica se uma máquina pode imitar o comportamento humano com sucesso.
- **Pensando racionalmente**: A IA busca seguir as leis da lógica e o raciocínio correto, como os **silogismos** de Aristóteles.
- **Agindo racionalmente**: O foco é em fazer com que um **agente** (entidade que percebe e atua no ambiente) tome a melhor decisão possível para atingir seus objetivos.

### 3. **Teste de Turing**
- Proposto por **Alan Turing** em 1950, o teste mede se uma máquina pode enganar uma pessoa, fazendo-a acreditar que está conversando com outro ser humano.
- Para passar no teste, a IA precisa de **processamento de linguagem natural**, **raciocínio automático** e **aprendizado de máquina**.

### 4. **Agente Racional**
- Um **agente racional** age para **maximizar o sucesso** com base nas informações disponíveis e nas ações mais adequadas ao seu objetivo.
- A racionalidade é limitada pelos **recursos computacionais** e pela complexidade do ambiente.

### 5. **História da IA**
- A IA começou com pesquisas em **modelos neurais artificiais** (McCulloch e Pitts, 1943) e ganhou força com o desenvolvimento de **sistemas especialistas** nas décadas de 60 e 70, como o **DENDRAL** e o **MYCIN**.
- Nas décadas de 80 e 90, a IA se tornou uma indústria com aplicações práticas, como sistemas de planejamento e diagnóstico.

### 6. **Objetivos da IA**
- **Científico**: Compreender os princípios que tornam o comportamento inteligente possível.
- **Engenharia**: Criar sistemas inteligentes úteis que possam aprender com a experiência e adaptar-se a mudanças no ambiente.

### 7. **Subáreas da IA**
- **Aprendizagem de máquina**: Como sistemas podem aprender com dados.
- **Percepção**: Visão computacional e processamento de linguagem natural.
- **Raciocínio**: Planejamento, tomada de decisões e resolução de problemas.

  

**Aula 03 - AGENTES** 

### 1. **Definição de Agente**
- Um **agente** é qualquer entidade que percebe seu ambiente (sensores) e age sobre ele (atuadores).
  - **Exemplos**: 
    - Humano (olhos como sensores, braços e pernas como atuadores).
    - Robô (câmeras, sensores e motores).
    - Software (recebe dados, gera saídas, como em impressoras).

### 2. **Agentes Inteligentes**
- Agentes inteligentes usam informações para tomar decisões e agir de forma eficiente.
- Podem aprender com **experiências passadas** para melhorar o desempenho futuro.
  
### 3. **Tipos de Agentes**
- **Robôs**: Movimentam-se, reconhecem objetos, falam, e aprendem a partir de experiências (como evitar obstáculos).
- **Médicos** (agentes médicos): Usam observações (sintomas, exames) para diagnosticar e tratar doenças.
- **Interfaces com Usuários**: Apresentam informações e interagem com o usuário, aprendendo com o feedback.

### 4. **Domínios de Aplicação**
- **Robôs de Entrega**: Navegam em ambientes, entregam objetos e aprendem com o caminho percorrido.
- **Assistentes de Diagnóstico**: Ajudam a identificar falhas ou doenças, propondo soluções baseadas em sintomas.
- **Agentes Comerciais**: Compram produtos ou serviços online com base nas preferências do usuário.

### 5. **Tarefas Comuns dos Agentes**
- **Modelar o ambiente**: Construir modelos do mundo ao redor.
- **Raciocínio baseado em evidências**: Tomar decisões com base nas informações recebidas.
- **Aprender com a experiência**: Melhorar suas ações a partir de eventos anteriores.

### 6. **Racionalidade dos Agentes**
- Um agente **racional** deve:
  1. Maximizar seu sucesso baseado em objetivos.
  2. Usar o conhecimento que possui do ambiente.
  3. Analisar as percepções que recebeu até o momento.
  
- A **racionalidade limitada** ocorre quando um agente deve tomar decisões com recursos limitados (tempo ou informação).

### 7. **Autonomia**
- Um agente **autônomo** aprende com o ambiente e ajusta seu comportamento, sem depender exclusivamente do conhecimento programado por seu criador.
  
### 8. **Problemas Complexos**
- Problemas enfrentados por agentes variam em complexidade. Quanto maior a **observabilidade** (o que o agente pode "ver"), mais fácil é para ele tomar decisões.

### 9. **Exemplo Clássico: Aspirador de Pó Inteligente**
- O agente precisa limpar uma sala, movendo-se de um ponto a outro, tomando decisões com base no que percebe (se a sala está suja ou não) e aprendendo como agir melhor.

Focar nesses conceitos principais vai te ajudar a entender como agentes inteligentes funcionam e aplicá-los em diferentes cenários.



**Aula 04 - Arquiteturas de Agentes e Controle Hierárquico**

### 1. **Sistema de Agentes**
- Um **agente** interage com o **ambiente** ao receber estímulos (sensores) e executar ações (atuadores).
- O agente é composto por um **corpo** (sensores e atuadores) e um **controlador** (cérebro que processa as percepções e envia comandos).

### 2. **Controlador do Agente**
- O controlador é o "cérebro" do agente, responsável por processar informações e tomar decisões.
- Ele recebe percepções e envia comandos ao corpo.
- O controlador age com **memória limitada** e **recursos computacionais limitados**.

### 3. **Transdução Causal**
- Refere-se ao processo de transformação das percepções do agente em comandos. 
- A decisão de uma ação no tempo t depende das percepções até aquele momento.

### 4. **Estado de Crença**
- Representa o que o agente **lembra** do passado e usa essas informações para guiar suas ações futuras.
- O **estado de crença** encapsula o histórico acessível ao agente.

### 5. **Controle Hierárquico**
- Em vez de três módulos independentes, uma arquitetura eficiente é o **controle hierárquico**.
  - Controladores de **nível inferior** reagem rapidamente ao mundo.
  - Controladores de **nível superior** gerenciam tarefas mais complexas.

### 6. **Exemplo: Robô de Entregas**
- O robô executa ações como seguir em frente, virar à esquerda ou direita, e evitar obstáculos com sensores simples.
- Controladores de nível superior definem o objetivo (local de entrega), enquanto controladores de nível inferior reagem a obstáculos no caminho.

### 7. **Agentes Simulados vs. Embutidos**
- **Agentes simulados** são usados em ambientes de teste (simulação), permitindo depuração antes de serem colocados em ambientes reais.
- **Agentes embutidos** operam diretamente no mundo real.

### 8. **Agindo com Raciocínio**
- Um sistema baseado em conhecimento (**Knowledge-Based System**) usa informações do domínio para tomar decisões e resolver problemas.
- O conhecimento é armazenado na **base de conhecimento** (memória de longo prazo) e atualizado com novas informações.
