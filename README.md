# Séries e Transformadas de Fourier: Remoção de Ruído de Áudio Usando a Transformada de Fourier

Este projeto visa desenvolver um sistema para remover ruídos em sinais de áudio usando a Transformada de Fourier. O método baseia-se na transformação do sinal do domínio do tempo para o domínio da frequência, onde componentes indesejáveis (ruídos) podem ser identificados e filtrados.

## Visão Geral do Projeto
- **Objetivo:** Utilizar a Transformada de Fourier para identificar e remover ruídos de áudios no domínio da frequência, retornando um sinal "limpo" no domínio do tempo. 
- **Conjunto de Dados:** O projeto inclui áudios curtos como exemplos para ilustrar as transformações e e reconstruir o sinal no domínio do tempo após a filtragem.
  
## Tecnologias Utilizadas
- Python
- NumPy
- Scipy
- Matplotlib
- Pydub
  
## Como Usar
1. Clone o repositório.
   ```bash
   https://github.com/larissa-maciel/Audio_Noise_Removal_Using_Fourier_Transform.git

2. Execute o notebook Jupyter localmente ou no Google Colab.

3. Carregue o conjunto de dados (áudios) e referencie o caminho correto no notebook.

4. Execute todas as células do notebook para visualizar e gerar as análises.
   
## Destaques

- **Carregamento e Normalização dos Sinais:** Utilização de pydub para carregar áudios em formato MP3 e convertê-los para arrays de dados, permitindo a manipulação direta. A normalização foi aplicada para ajustar as amplitudes entre -1 e 1, garantindo consistência na comparação de sinais.
- **Transformada de Fourier (FFT):** Implementação da FFT para converter o sinal de áudio para o domínio da frequência, onde foi possível visualizar as frequências dominantes e identificar componentes de ruído.
- **Filtragem de Ruído com Filtro Passa-Baixas:** A partir da análise de frequências, foi implementado um filtro passa-baixas para atenuar componentes acima de uma frequência de corte específica, eliminando ruídos de alta frequência.
- **Reconstrução do Sinal com a Transformada Inversa de Fourier (IFFT):** Após a filtragem, o sinal foi reconstruído no domínio do tempo usando a IFFT, resultando em um áudio "limpo".

A Transformada de Fourier, combinada com filtros no domínio da frequência, demonstrou ser uma técnica eficaz para remoção de ruídos em sinais de áudio. Este projeto mostrou que, ao aplicar filtros adequados, é possível isolar componentes de ruído de modo eficaz. Esta abordagem abre possibilidades para aprimoramentos, como o uso de filtros passa-altas e passa-banda para tratar diferentes tipos de ruído em futuros experimentos.
