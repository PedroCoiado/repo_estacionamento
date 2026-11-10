# 🚗 Sistema de Gestão de Estacionamento

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python&logoColor=white)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-success?style=for-the-badge)

Um sistema de gerenciamento de estacionamento via terminal (CLI) desenvolvido em Python. O projeto foi construído para mapear a ocupação de vagas, gerenciar entradas e saídas de veículos, alocar vagas PCD e persistir dados de forma leve e eficiente.

Este projeto foi desenvolvido como um trabalho acadêmico do curso de Ciência da Computação (UNICID), onde atuei como líder de uma equipe de 9 pessoas no 1º semestre (Maio de 2026).

## ✨ Funcionalidades

*   **Mapa de Ocupação em Tempo Real:** Visualização dinâmica das vagas (1 a 15), mostrando quais estão livres, ocupadas ou reservadas.
*   **Validação de Placas (Regex):** Suporte nativo para validação de placas brasileiras tanto no padrão antigo (ABC1234) quanto no padrão Mercosul (ABC1D23).
*   **Vagas Exclusivas (PCD):** Lógica de bloqueio e verificação para vagas designadas a Pessoas com Deficiência (ex: Vaga 1).
*   **Persistência em JSON:** O estado do estacionamento é salvo automaticamente no arquivo `Dados.json`. Se o programa for fechado, os carros continuam lá ao reabrir.
*   **Sistema de Auditoria (Logs):** Registro silencioso de eventos do sistema em um arquivo `estacionamento.log` para monitoramento.
*   **Simulação de Risco de Colisão:** Algoritmo de probabilidade que calcula o risco (15% ou 35%) de um "esbarrão" ao estacionar dependendo da presença de carros nas vagas vizinhas.

## 🛠️ Tecnologias e Bibliotecas

O projeto foi construído 100% com **Python puro**, utilizando apenas módulos embutidos na linguagem:
*   `json` - Para leitura e gravação do banco de dados local.
*   `logging` - Para a geração de logs de eventos e auditoria.
*   `re` - Expressões regulares para a validação das placas dos veículos.
*   `random` - Geração de números aleatórios para o algoritmo de colisão.
*   `os` - Verificação de existência de arquivos no sistema operacional.

## 🚀 Como Executar

### Pré-requisitos
*   Ter o [Python 3.x](https://www.python.org/downloads/) instalado na sua máquina.

### Passo a Passo

1. Clone este repositório para a sua máquina local:
   ```bash
   git clone [https://github.com/SEU_USUARIO/sistema-gestao-estacionamento.git](https://github.com/SEU_USUARIO/sistema-gestao-estacionamento.git)
