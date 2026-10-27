# Лабораторная работа 1. Дискретное пространство состояний

Обучение с подкреплением на среде [RedBlueDoorEnv](https://minigrid.farama.org/environments/minigrid/RedBlueDoorEnv/) из MiniGrid (конфигурация `MiniGrid-RedBlueDoors-6x6-v0`). Агент должен открыть сначала красную дверь, затем синюю.

Задание — в [task.md](task.md) (оригинал — `ЛР1.docx`).

## Содержание

| Файл | Что внутри |
|---|---|
| [lab01.ipynb](lab01.ipynb) | Решение: код, картинки, графики и пояснения по пунктам задания |
| [task.md](task.md), `ЛР1.docx` | Текст задания |
| `seminar_vi.ipynb`, `crossentropy_method.ipynb`, `homework.ipynb` | Шаблоны из курса [Practical_RL](https://github.com/yandexdataschool/Practical_RL), код из которых адаптируется в решении |

### Прогресс

- [x] 1. Знакомство со средой, `FullyObsWrapper`, `BinaryRewardWrapper`
- [x] 2. Ручной расчёт трёх итераций уравнения Беллмана
- [x] 3. Value iteration для функции ценности состояний
- [x] 4. Метод кросс-энтропии
- [x] 5. Q-learning
- [ ] 6. SARSA и Expected Value SARSA (softmax), сравнение с Q-learning

## Запуск

Нужен Python 3.12 (или 3.11).

```bash
python -m venv .venv
# Windows: .venv\Scripts\activate    Linux/macOS: source .venv/bin/activate
pip install gymnasium minigrid numpy matplotlib pandas tqdm ipykernel jupyter
jupyter lab lab01.ipynb
```

Проверенные версии: gymnasium 1.4.0, minigrid 3.2.0.

Выполнить ноутбук целиком без интерфейса (выходы сохраняются в файл):

```bash
jupyter nbconvert --to notebook --execute --inplace lab01.ipynb
```
