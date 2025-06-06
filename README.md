# 🔥 HeatMap – Sistema Inteligente de Combate a Queimadas

👨‍💻 **Autores:** Matheus Farias (RM554254) & Miguel Parrado (RM554007)  
📘 **Disciplina:** Estrutura de Dados | FIAP  
📌 **Tema Global Solution:** Prevenção e Resposta a Incêndios Florestais

---

## 📖 Sobre o Projeto

O **HeatMap** é uma simulação de uma central de emergência florestal, que toma decisões automatizadas sobre:

- 🚨 Quais focos atender primeiro  
- 🗺️ Qual caminho seguir até o local do incêndio  
- 👷 Qual equipe será designada  
- 🧯 Quais ações serão tomadas  
- 📈 Como atualizar o status das áreas afetadas

Tudo isso usando **estruturas de dados clássicas** aplicadas de forma prática e integrada.

---

## 🧠 Funcionalidades

✅ Receber e organizar as chamadas em tempo real (Queue)  
✅ Repriorizar ocorrências com base na severidade (Heap)  
✅ Registrar ações de combate a incêndios (Stack)  
✅ Traçar rotas com menor tempo usando Dijkstra (Graph)  
✅ Atualizar o status da área afetada dinamicamente (Linked List)  
✅ Simular hierarquia regional com árvore (Tree)  
✅ Exibir relatório completo por ocorrência

---

## 🧱 Estruturas Utilizadas

| Estrutura de Dados | Aplicação no HeatMap |
|--------------------|----------------------|
| 🟦 Fila (Queue)     | Ordem de chegada das chamadas |
| 🟨 Heap de Prioridade | Priorização por severidade e vegetação |
| 🟥 Pilha (Stack)     | Registro das ações realizadas |
| 🟩 Lista Ligada      | Status dinâmico das áreas afetadas |
| 🌳 Árvore (Tree)     | Hierarquia geográfica: Estado → Município → Zona |
| 🔄 Grafo (Graph)     | Mapa com distâncias entre os locais (Dijkstra) |

---

## 🗺️ Exemplo de Grafo

```python
mapa = {
  "Base Central": {"Zona Norte": 10, "Vila Verde": 5},
  "Zona Norte": {"Base Central": 10, "Mata Alta": 7},
  "Vila Verde": {"Base Central": 5, "Mata Alta": 3},
  "Mata Alta": {"Zona Norte": 7, "Vila Verde": 3}
}
```

---

## 🔁 Chamadas Simuladas

```python
chamadas = [
  {"id": 1, "local": "Zona Norte", "severidade": 4, "tipo_vegetacao": "cerrado"},
  {"id": 2, "local": "Mata Alta", "severidade": 5, "tipo_vegetacao": "pantanal"},
  {"id": 3, "local": "Vila Verde", "severidade": 3, "tipo_vegetacao": "mata_atlantica"}
]
```

---

## ⚙️ Execução

1. 📥 Faça o download do arquivo: `GS-DYNAMIC PROGRAMMING.ipynb`
2. ✅ Execute no [Google Colab](https://colab.research.google.com/), Jupyter Notebook ou ambiente local com Python 3+
3. 📊 Observe as simulações, relatórios e decisões impressas diretamente

---

## 🧾 Resultados Esperados

Para cada ocorrência, o sistema retorna:

- ID da ocorrência  
- Prioridade calculada  
- Equipe designada  
- Rota otimizada até o foco  
- Tempo estimado  
- Ações realizadas  
- Status atualizado da área

---

## 🏁 Conclusão

O HeatMap demonstra com clareza como as estruturas de dados são aplicáveis a cenários reais e críticos, promovendo agilidade, eficiência e rastreabilidade em decisões de emergência ambiental.

Este projeto cumpre todos os requisitos propostos pela disciplina, com código comentado, modular, e foco em boas práticas.

---

## 📝 Licença

Projeto de uso acadêmico. Todos os direitos reservados aos autores.
