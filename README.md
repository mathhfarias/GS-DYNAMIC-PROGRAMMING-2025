
````markdown
# 🔥 HeatMap – Sistema Inteligente de Combate a Queimadas

**Autores:** Matheus Farias (RM554254) e Miguel Parrado (RM554007)  
**Disciplina:** Estrutura de Dados / Global Solution  
**Tema:** Prevenção e Resposta a Incêndios

---

## 📘 Descrição

O **HeatMap** é um sistema de simulação que representa o funcionamento de uma **central de emergência ambiental**. Ele utiliza estruturas de dados clássicas e técnicas de programação dinâmica para tomar decisões inteligentes no combate a focos de incêndio.

Este projeto foi desenvolvido como parte da avaliação acadêmica da disciplina de Estrutura de Dados, com o objetivo de demonstrar a aplicação prática de conceitos como:

- Fila (FIFO)
- Heap de prioridade
- Pilha (LIFO)
- Lista ligada
- Árvore de regiões
- Grafos e o algoritmo de Dijkstra

---

## 🧠 Funcionalidades

- ✅ Receber chamadas de emergência em tempo real (fila FIFO)
- ✅ Reordenar chamadas com base em prioridade (heap de prioridade)
- ✅ Traçar o caminho mais curto até o foco (algoritmo de Dijkstra)
- ✅ Registrar ações tomadas em cada ocorrência (pilha)
- ✅ Atualizar dinamicamente o status das áreas afetadas (lista ligada)
- ✅ Representar hierarquia geográfica (árvore de regiões)
- ✅ Exibir relatório completo por ocorrência

---

## 📊 Estruturas Utilizadas

| Estrutura         | Implementação |
|------------------|----------------|
| Fila (Queue)      | `CallQueue` com `collections.deque` |
| Heap de Prioridade | `PriorityHeap` com `heapq` |
| Pilha (Stack)     | `ActionStack` com lista |
| Lista Ligada      | `AreaLinkedList` com `AreaNode` |
| Árvore            | `RegionTree` |
| Grafo             | `dict` aninhado + Dijkstra |

---

## 🗺 Exemplo de Mapa (Grafo)

```python
mapa = {
    "Base Central": {"Zona Norte": 10, "Vila Verde": 5},
    "Zona Norte": {"Base Central": 10, "Mata Alta": 7},
    "Vila Verde": {"Base Central": 5, "Mata Alta": 3},
    "Mata Alta": {"Zona Norte": 7, "Vila Verde": 3}
}
````

---

## 🔁 Simulação de Chamadas

```python
chamadas = [
    {"id": 1, "local": "Zona Norte", "severidade": 4, "tipo_vegetacao": "cerrado"},
    {"id": 2, "local": "Mata Alta", "severidade": 5, "tipo_vegetacao": "pantanal"},
    {"id": 3, "local": "Vila Verde", "severidade": 3, "tipo_vegetacao": "mata_atlantica"}
]
```

---

## ✅ Como executar

1. Baixe o notebook (./GS-DYNAMIC PROGRAMMING.ipynb)
2. Execute em qualquer ambiente Jupyter, JupyterLab ou Google Colab
3. Verifique os relatórios e resultados impressos diretamente no console

---

## 📌 Conclusão

O HeatMap demonstra como estruturas de dados podem ser aplicadas na vida real para resolver problemas críticos de logística e resposta emergencial. Através de uma simulação compacta e interativa, o projeto atende a todos os critérios propostos pelo professor e vai além ao incorporar modularidade e clareza no código.

---

## 🧾 Licença

Uso acadêmico. Todos os direitos reservados aos autores.

```
