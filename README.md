# Gestão de Processos Seletivos para Docentes

Aplicação **desktop desenvolvida em Java com JavaFX**, criada para simular a gestão de **processos seletivos de professores temporários** em um contexto acadêmico.

O projeto tem como foco demonstrar habilidades práticas em **Programação Orientada a Objetos**, **estruturas de dados**, **organização de código** e **persistência de informações**, aproximando-se de cenários reais do desenvolvimento de software.

---

## 🎯 Objetivo

Automatizar e centralizar o controle de:
- Disciplinas ofertadas
- Docentes candidatos
- Inscrições em processos seletivos

Garantindo integridade dos dados, consultas eficientes e facilidade de manutenção.

---

## 🛠️ Funcionalidades

- Gerenciamento de entidades acadêmicas (cursos, disciplinas e docentes)
- Controle de inscrições em processos seletivos
- Classificação de candidatos com base em pontuação
- Consulta de processos seletivos ativos
- Interface gráfica desenvolvida com JavaFX
- Persistência de dados utilizando arquivos CSV

---

## 🧠 Regras e Lógica de Negócio

- Apenas docentes previamente cadastrados podem se inscrever em disciplinas
- Exclusões mantêm a consistência dos dados (remoções em cascata quando aplicável)
- Operações de alteração utilizam estruturas encadeadas
- Consultas são realizadas a partir de estruturas auxiliares carregadas dos arquivos
- Os arquivos de dados permanecem consistentes após qualquer operação

---

## 🧮 Estruturas de Dados e Algoritmos

O sistema utiliza conceitos fundamentais de Estrutura de Dados:

- Listas encadeadas
- Filas
- Tabelas hash
- Algoritmo de ordenação QuickSort

Esses recursos foram aplicados visando desempenho, clareza e organização.

---

## 🧱 Organização do Projeto

A aplicação segue uma estrutura inspirada no padrão **MVC**, promovendo separação de responsabilidades:

- **Domínio**: entidades do sistema
- **Controle**: regras de negócio e validações
- **Interface**: telas e interação com o usuário
- **Persistência**: leitura e escrita de dados em CSV

Essa abordagem facilita manutenção e evolução do sistema.

---

## ▶️ Como Executar

1. Importe o projeto em uma IDE compatível com Java
2. Adicione as bibliotecas auxiliares ao classpath
3. Execute a classe principal da aplicação

Os arquivos CSV são gerados automaticamente na primeira execução.

---

## 💡 Observações Técnicas

- Interface gráfica construída com JavaFX
- Armazenamento local de dados em formato CSV
- Tratamento de erros com feedback visual ao usuário
- Atualização automática da interface após operações
- Código organizado com foco em legibilidade e boas práticas

---

Este projeto demonstra capacidade de **modelar soluções**, **aplicar fundamentos da computação** e **desenvolver aplicações desktop bem estruturadas**, sendo adequado para fins acadêmicos e apresentação profissional.
