# Maquina-de-Turing-Parelela
Autores
Pedro Arthur da Silva Guimarães

Leonardo Abreu Ferreira

Descrição do Projeto
Este projeto implementa uma Máquina de Turing Paralela que realiza a ordenação de elementos em uma fita utilizando duas cabeças de leitura/escrita simultâneas. A máquina simula um algoritmo de ordenação do tipo bubble sort paralelizado, onde cada cabeça opera em uma metade da fita, permitindo comparações e trocas simultâneas.

Funcionalidades
Ordenação Paralela: Utiliza duas cabeças para percorrer e ordenar metades diferentes da fita simultaneamente.

Visualização Interativa: Gera uma animação que mostra o passo a passo da ordenação, incluindo comparações e trocas realizadas.

Registro de Passos: Mantém um histórico detalhado de cada operação realizada durante a ordenação.

Como Executar
Pré-requisitos:

Python 3.x instalado.

Bibliotecas necessárias: matplotlib.

Instalação das Dependências:

bash
pip install matplotlib
Execução:

Execute o script turing_machine_parallel.py em um ambiente Python ou em um notebook Jupyter/Colab.

A animação será exibida automaticamente após a execução.

Exemplo de Uso
python
# Fita inicial com elementos a serem ordenados
fita_inicial = ['9', '3', '7', '5', '2', '8', '4', '1', '6', '0']
mt = TuringMachineParallel(fita_inicial)
quadros = mt.executar()

# A animação será gerada automaticamente
Saída Esperada
Uma animação interativa que mostra:

A fita dividida em duas metades (Fita 1 e Fita 2).

As posições das cabeças de leitura/escrita durante cada passo.

As operações realizadas (comparações, trocas) e o estado atual da máquina.

Estrutura do Código
Classe TuringMachineParallel:

__init__: Inicializa a máquina com a fita fornecida.

registrar: Armazena o estado atual para visualização.

passo: Executa um único passo da ordenação paralela.

executar: Roda a máquina até a conclusão da ordenação.

Visualização:

Utiliza matplotlib para criar a animação passo a passo.

Contribuições
Este projeto foi adaptado para funcionar em paralelo a partir de um projeto já existente, conforme solicitado pelo professor. As principais adaptações incluem:

Implementação de duas cabeças de leitura/escrita.

Lógica de ordenação paralela entre as metades da fita.

Geração da animação para visualização do processo.
