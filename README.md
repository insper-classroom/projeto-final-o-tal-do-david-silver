# 🧠 Curriculum Learning em Ambientes de Reinforcement Learning

## 📌 Objetivo do Projeto

Este projeto tem como objetivo investigar os efeitos da introdução de **Curriculum Learning (CL)** no processo de aprendizado por reforço. A proposta central é comparar o desempenho de agentes treinados com e sem o uso de um currículo progressivo de tarefas, avaliando o impacto sobre métricas relevantes como:

- ⏱️ **Tempo de convergência**
- 🎯 **Valor da recompensa na convergência**
- 🎲 **Entropia da política durante o treinamento**

## 🎓 O que é Curriculum Learning?

Curriculum Learning é uma estratégia de treinamento inspirada na forma como humanos aprendem: começando por tarefas simples e progredindo para tarefas mais complexas. No contexto de RL, isso pode significar começar com versões mais fáceis de um ambiente e gradualmente aumentar sua complexidade à medida que o agente melhora.

## 🔬 Metodologia

1. **Seleção de Ambientes**  
   Vamos selecionar alguns ambientes clássicos, como:
    - LunarLander-v2
    - MiniGridWorld
    ...

2. **Definição dos Currículos**  
   Para cada ambiente, vamos estudar quais aspectos vamos quebrar em partes menores (a avaliação faz parte do projeto).

3. **Arquitetura do Agente**  
   Os agentes utilizam algoritmos clássicos de RL como:
   - DQN
   - PPO
   - A2C  
   (Dependendo da configuração experimental, via de regra, o PPO é o mais utilizado.)

4. **Experimentos Comparativos**  
   Para cada ambiente:
   - Treinamento com currículo progressivo
   - Treinamento direto (sem currículo)
   - Análise quantitativa das métricas definidas

## 📈 Métricas Avaliadas

- **Tempo de convergência**: Número de episódios até estabilização da recompensa média.
- **Recompensa final**: Valor médio da recompensa nas últimas N iterações.
- **Entropia da política**: Avaliação da aleatoriedade das decisões ao longo do tempo (quanto menor, mais determinística a política).

## 🧪 Resultados Esperados

A hipótese é que o uso de curriculum learning:
- Reduzirá o tempo de convergência,
- Permitirá alcançar recompensas mais altas (melhor política final),
- Promoverá políticas menos aleatórias, com entropia decrescente de forma mais estável.

## ⚙️ Requisitos

- Gymnasium ou Gym
- NumPy, Matplotlib, pandas
- Stable-Baselines3 (ou outra biblioteca de RL)
- Tensorboard


[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/bFrIHgJ3)
