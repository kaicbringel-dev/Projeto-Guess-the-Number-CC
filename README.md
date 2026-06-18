# Projeto-Guess-the-Number-CC
"Guess the Number" é um projeto para a disciplina de Circuitos Digitais desenvolvido no Logisim. Universidade Federal do Cariri
**Disciplina:** Circuitos Digitais | UFCA
**Professor:** Ramon Nepomuceno

## Sobre o projeto
Sistema de **adivinhação de números binários** aleatórios de 4 bits desenvolvido no **Logisim**. O circuito avalia o palpite do jogador, calcula a distância em relação ao valor correto e fornece a distância baseada na intensidade das cores **vermelha** (perto) e **azul** (longe).  

  ## Desenvolvimento
Implementação do circuito `circuito_diferenca`. <br>
Implementação do circuito `circuito_comparador`. 

## - Circuitos 2/4

### I. Circuito "Diferença"

* **Premissa:** Calcular a distância $|A - B|$ entre o chute do usuário e a resposta.
   
* **Componentes:**  
    * 2 subtratores de 4 bits feitos manualmente, um para A-B, outro para B-A.
    * 1 Multiplexador (MUX) manual 2x1 para seleção do resultado positivo $|A - B|$.
    * 3 pinos: Escolha do Usuário, da CPU e Distância.
        
* **Desafios/Bugs**
   

<details>
  <summary><a href="#diferenca">Clique para abrir a imagem do Subcircuito Diferenca</a></summary>
  <br>
  
  ![Circuito Diferença]()
</details>

<br>
<br>

### II. Circuito "Comparador"

* **Premissa:** Verificar a possível igualdade entre o número A e B.
   
* **Componentes:**
  **Opção 1:**
  * 8 pinos de Entrada: A1-A2-A3-A4 e B1-B2-B3-B4.
  * 4 portas XNOR para compara se A1 = B1; A2 = B2; A3 = B3; A4 = B4.
  * 1 porta AND para comparar se todos são iguais.
  * 1 porta de Saída (S) para dizer se é igual(1) ou não(0).
 
  **Opção 2:**
  * 2 pinos de Entrada de 4 bits (A e B).
  * 2 distribuidores de 4 bits de entrada e saída.
  * 4 portas XNOR para comparar os valores.
  * 1 porta AND para comparar se todos são iguais.
  * 1 porta de Saída (S) para dizer se é igual(1) ou não(0).
        
* **Desafios/Bugs**
    <p>Nenhum.</p>

<details>
  <summary><a href="#comparador">Clique para abrir a imagem do Subcircuito Comparador</a></summary>
  <br>
<img width="988" height="684" alt="comparador" src="https://github.com/user-attachments/assets/6c009fa0-7e8d-4b29-9977-81af88f846fd" />
</details>
    
<br>
<br>

## II.I . Circuito de Comparador de Magnitude

* **Premissa:** Verificar se A = B ou A > B ou A < B

* **Componentes:**
  * 8 pinos de entrada A1;A2;A3;A4;B1;B2;B3;B4.
  * 4 portas XNOR
  * 4 portas NOT
  * 5 portas AND
  * 1 portas OR
  * 1 porta NOR
 
<details>
  <summary><a href="#comparador">Clique para abrir a imagem do Subcircuito Comparador</a></summary>
  <br>
<img width="1692" height="1390" alt="image" src="https://github.com/user-attachments/assets/f2568cd8-26ca-4d82-9ffd-652116cf9238" />
</details>
    
<br>
<br>

