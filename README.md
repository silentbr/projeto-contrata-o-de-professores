# Sistema de Contratação de Docente

Aplicação desenvolvida em **Java com JavaFX**, simulando um sistema real de **gestão de contratação temporária de docentes** em uma instituição de ensino superior.  
O projeto demonstra domínio de **Programação Orientada a Objetos**, **estruturas de dados**, **organização em camadas** e **persistência de dados em arquivos CSV**.

---

## 📌 Funcionalidades

### 🔧 CRUD Completo
- **Cursos**: Cadastro, busca, atualização e remoção  
- **Disciplinas**: Gerenciamento de disciplinas vinculadas a cursos  
- **Professores**: Cadastro de docentes com pontuação classificatória  
- **Inscrições**: Controle de inscrições em processos seletivos  

### 🔍 Consultas Estratégicas
- **Consulta de Inscritos**: Lista professores inscritos por disciplina, ordenados por pontuação utilizando **QuickSort**  
- **Processos Abertos**: Exibe disciplinas com processos seletivos ativos usando **HashTable**  

---

## 📁 Estrutura do Projeto

```text
/contratacao-docente
├── csv/
│   ├── disciplinas.csv
│   ├── cursos.csv
│   ├── professores.csv
│   └── inscricoes.csv
│
├── doc/
│   └── diagrama.png
│
├── lib/
│   ├── ListaSimples.jar
│   ├── Fila.jar
│   └── HashTable.jar
│
├── src/
│   ├── application/
│   │   └── MainApp.java
│   │
│   ├── controller/
│   │   ├── CursoController.java
│   │   ├── DisciplinaController.java
│   │   ├── ProfessorController.java
│   │   └── InscricaoController.java
│   │
│   ├── persistence/
│   │   ├── CursoRepository.java
│   │   ├── DisciplinaRepository.java
│   │   ├── ProfessorRepository.java
│   │   └── InscricaoRepository.java
│   │
│   ├── model/
│   │   ├── Curso.java
│   │   ├── Disciplina.java
│   │   ├── Professor.java
│   │   └── Inscricao.java
│   │
│   ├── view/
│   │   ├── CursoView.java
│   │   ├── DisciplinaView.java
│   │   ├── ProfessorView.java
│   │   ├── InscricaoView.java
│   │   ├── ConsultaInscritos.java
│   │   └── ConsultaProcessosAbertos.java
│   │
│   └── util/
│       └── QuickSort.java
```

---

## 🧩 Regras de Negócio

1. Apenas professores previamente cadastrados podem realizar inscrições  
2. A remoção de uma disciplina exclui automaticamente todas as inscrições relacionadas  
3. Operações de atualização e remoção utilizam **listas encadeadas**  
4. Consultas de dados utilizam **filas** carregadas a partir dos arquivos CSV  
5. Os arquivos CSV são mantidos consistentes, sem linhas vazias após operações  

---

## 📚 Estruturas de Dados Utilizadas

- Lista Simples Encadeada  
- Fila  
- QuickSort  
- HashTable  

---

## ▶️ Como Executar

1. Verifique se as bibliotecas estão disponíveis na pasta `lib/`  
2. Adicione as bibliotecas ao **Build Path** do projeto  
3. Execute a classe **MainApp.java**  

---

## 🏗️ Arquitetura

O sistema segue um **MVC bem definido**, facilitando manutenção e escalabilidade:

- **Model**: Entidades de domínio  
- **View**: Interface gráfica desenvolvida em JavaFX  
- **Controller**: Regras de negócio e fluxo da aplicação  
- **Persistence**: Repositórios responsáveis pelo acesso aos arquivos CSV  

---

## ⚙️ Observações Técnicas

- Arquivos CSV criados automaticamente na pasta `csv/`  
- Separador CSV: `;`  
- Quebra de linha: `\r\n`  
- Mensagens de erro tratadas com `AlertDialog`  
- Resultados de consultas exibidos em `TextArea`  
- Campos de entrada são limpos após cada operação  
