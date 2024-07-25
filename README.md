import random

# Dicionário de perguntas e respostas
questions = [
    {
        "question": "Qual é a capital do Brasil?",
        "options": ["Rio de Janeiro", "São Paulo", "Brasília"],
        "answer": "Brasília"
    },
    {
        "question": "Quem escreveu 'Dom Quixote'?",
        "options": ["Miguel de Cervantes", "William Shakespeare", "Jorge Luis Borges"],
        "answer": "Miguel de Cervantes"
    },
    {
        "question": "Quanto é 2 + 2?",
        "options": ["3", "4", "5"],
        "answer": "4"
    }
]

def display_question(question):
    print(question["question"])
    for i, option in enumerate(question["options"], start=1):
        print(f"{i}. {option}")
    print()

def play_game():
    score = 0
    random.shuffle(questions)  # Embaralha as perguntas

    for question in questions:
        display_question(question


