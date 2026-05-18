# Projeto

## 📌 Estrutura do Sistema

O sistema será dividido em múltiplas classes responsáveis por partes específicas da aplicação, utilizando o reaproveitamento de código para otimizar a arquitetura do jogo.

---

## 🧱 Classes

### Character
Classe base abstrata do sistema. Graças ao pilar da POO, ela é utilizada tanto para estruturar os Heróis quanto para o **reaproveitamento de código na criação do Chefão**, evitando a necessidade de criar uma classe exclusiva para o inimigo.

Responsável por encapsular:
- Nome
- Vida (HP atual e máximo)
- Poder de Ataque

---

### Warrior
Classe derivada de Character por herança.
Características: Alta resistência (HP elevado) e dano físico moderado.

---

### Mage
Classe derivada de Character por herança.
Características: Alta capacidade ofensiva (Ataque mágico elevado) e menor resistência.

---

### Archer
Classe derivada de Character por herança.
Características: Atributos balanceados entre vida e dano de longo alcance.

---

### QuestionManager
Responsável por:
- Armazenar o banco de perguntas.
- Sorteá-las e validar qual alternativa clicada é a correta.

---

### MainWindow
Classe que gerencia o ciclo de vida e turnos do combate (Associação). Ela instancia o Herói selecionado e o Chefão (reutilizando a estrutura de `Character`), alterando os elementos gráficos da interface a cada rodada.

---

## 🧠 Herança

```text
Character (Utilizada para Heróis e também reutilizada para o Chefão)
 ├── Warrior
 ├── Mage
 └── Archer
