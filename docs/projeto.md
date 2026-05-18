# Projeto

## 📌 Estrutura do Sistema

O sistema será dividido em múltiplas classes responsáveis por partes específicas da aplicação.

---

## 🧱 Classes

### Character
Classe base abstrata do sistema.

Responsável por:
- Encapsular Nome, Vida (HP) e Poder de Ataque.
- Definir o método virtual puro de ataque (Polimorfismo).

---

### Warrior
Classe derivada de Character (Herança).

Características:
- Alta resistência (HP elevado) e dano físico moderado.

---

### Mage
Classe derivada de Character (Herança).

Características:
- Alta capacidade ofensiva (Grande dano mágico) e menor resistência.

---

### Archer
Classe derivada de Character (Herança).

Características:
- Atributos equilibrados entre vida e dano.

---

### QuestionManager
Responsável por:
- Armazenar e gerenciar o banco de perguntas do quiz.
- Validar as respostas selecionadas pelo jogador.

---

### MainWindow
Responsável por:
- Gerenciar a interface gráfica (Qt Widgets) e as abas do jogo.
- Controlar o fluxo dos turnos da batalha (Associação com as classes de personagens).

---

## 🧠 Herança

```text
Character
 ├── Warrior
 ├── Mage
 └── Archer
