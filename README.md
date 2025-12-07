# WumpusTheGame_JAVA
ENG Descripion - A Java implementation of the classic "Wumpus World" game developed for the final project of OOP course. Features a GUI - Guided User Interface elaborated with (JAVA-Swing), inventory management, crafting mechanics, and custom enemy behaviors.
# 🏹 O Mundo de Wumpus - Projeto Final POO

> Trabalho final desenvolvido para a disciplina de Programação Orientada a Objetos (Java).

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![Status](https://img.shields.io/badge/Status-Concluído-green?style=for-the-badge)

## 📄 Sobre o Projeto

Este projeto é uma releitura do clássico jogo **"O Mundo de Wumpus"**, onde o jogador controla um agente em uma caverna escura (tabuleiro 15x15) repleta de perigos. O objetivo é encontrar o Ouro e retornar à saída sem ser devorado pelos monstros ou cair em abismos.

O diferencial desta versão inclui a gestão de inventário, uso de lanterna, coleta de madeira para tapar buracos e a existência de dois tipos de monstros com comportamentos distintos.

## 🎮 Funcionalidades e Regras

O jogo implementa as seguintes mecânicas baseadas na especificação do trabalho:

* **Tabuleiro 15x15:** O mapa começa oculto e é revelado conforme a exploração.
* **Percepções Sensoriais:**
    * 🌬️ **Brisa:** Indica que há um poço (abismo) em uma casa adjacente.
    * 🧟 **Fedor:** Indica que um Wumpus está por perto.
* **Inimigos:**
    * **Wumpus Clássico:** Move-se uma casa por vez.
    * **Monstro Rápido:** Move-se em "L" (como o cavalo do Xadrez) e é mais agressivo.
* **Inventário do Jogador:**
    * 🏹 **Arco e Flecha:** Para eliminar monstros (alcance limitado).
    * 🪵 **Madeira:** Pode ser coletada e usada para criar flechas ou tapar poços.
    * 🔦 **Lanterna:** Ilumina uma direção até a borda do mapa (bateria limitada).
    * 💰 **Ouro:** O objetivo final do jogo.
* **Interface Gráfica:** Desenvolvida utilizando Java Swing.

## 🧩 Conceitos de POO Aplicados

Durante o desenvolvimento, foram aplicados os pilares da Orientação a Objetos:

* **Encapsulamento:** Uso de modificadores de acesso (`private`, `public`) e métodos `getters` e `setters` (ex: classe `Jogador`, `ItensInventario`).
* **Herança e Interfaces:** Implementação da interface `Personagem` para padronizar comportamentos entre o `Jogador` e os monstros (`MonstroLento`, etc).
* **Polimorfismo:** Tratamento genérico de objetos no tabuleiro.

## 🚀 Como Executar o Projeto

### Pré-requisitos
* Ter o **Java JDK** (versão 8 ou superior) instalado.
* Git (opcional, para clonar o repositório).

### 📂 Estrutura de Pastas Sugerida
Para que os comandos abaixo funcionem perfeitamente, certifique-se de que seus arquivos `.java` estejam dentro de uma pasta `src/jogo`. A estrutura deve ficar assim:

```text
MeuProjetoWumpus/
├── src/
│   └── jogo/
│       ├── Jogo.java
│       ├── Jogador.java
│       ├── Tabuleiro.java
│       ├── MonstroLento.java
│       └── ... (outros arquivos .java)
└── README.md
