- 👋 Hi, I’m @NATHONE
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
NATHONE/NATHONE is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import nltk
from nltk.chat.util import Chat, reflections

pairs = [
    [
        r"salut|bonjour",
        ["Salut", "Bonjour", "Comment ça va ?"]
    ],
    [
        r"ça va ?",
        ["Oui, ça va bien, et toi ?", "Je vais bien, merci."]
    ],
    [
        r"quel est ton nom ?",
        ["Je suis un assistant virtuel.", "Je n'ai pas de nom, je suis un programme informatique."]
    ],
    [
        r"quit",
        ["Au revoir, à bientôt !", "À la prochaine."]
    ]
]

def simple_chatbot():
    print("Bonjour ! Je suis un chatbot. Pose-moi des questions ou dis-moi bonjour.")
    chatbot = Chat(pairs, reflections)
    chatbot.converse()

if __name__ == "__main__":
    simple_chatbot()
    <!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulaire de soumission de questions</title>
</head>
<body>
    <h2>Formulaire de soumission de questions</h2>
    <form action="/submit-question" method="post">
        <div>
            <label for="question">Posez votre question :</label>
            <input type="text" id="question" name="question" required>
        </div>
        <div>
            <label for="email">Votre adresse e-mail :</label>
            <input type="email" id="email" name="email" required>
        </div>
        <div>
            <input type="submit" value="Soumettre">
        </div>
    </form>
</body>
</html>
