# Projeto

## 📌 Estrutura do Sistema

O sistema será dividido em múltiplas classes responsáveis por partes específicas da aplicação.

---

## 🧱 Classes

### Character
Classe base do sistema.

Responsável por:
- Nome
- Vida
- Ataque

---

### Warrior
Classe derivada de Character.

Características:
- Alto dano físico

---

### Mage
Classe derivada de Character.

Características:
- Ataque mágico

---

### Archer
Classe derivada de Character.

Características:
- Ataque balanceado

---

### QuestionManager
Responsável por:
- Gerenciar perguntas
- Validar respostas

---

## 🧠 Herança

```text
Character
 ├── Warrior
 ├── Mage
 └── Archer
