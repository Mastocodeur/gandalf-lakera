# 🛡️ Attaques sur LLM – Prompt Engineering appliqué à Gandalf (Lakera)


<p>
  <a href="PROMPTS.md" style="display:inline-block;padding:8px 16px;background-color:#1e90ff;color:#ffffff;border-radius:6px;text-decoration:none;">📜 Liste des techniques</a>
  &nbsp;&nbsp;&nbsp;
  <a href="SOLUTIONS.md" style="display:inline-block;padding:8px 16px;background-color:#28a745;color:#ffffff;border-radius:6px;text-decoration:none;">🧪 Mes solutions</a>
</p>



## 🧠 Qu’est-ce que le Prompt Engineering ?

Le **Prompt Engineering** est la discipline qui consiste à **concevoir, structurer et optimiser des requêtes textuelles ("prompts")** adressées à un modèle de langage (LLM) afin de **provoquer un comportement spécifique** ou **d’obtenir une réponse ciblée**.

Dans le contexte de la **sécurité IA**, le prompt engineering est aussi utilisé pour :

- ✅ Tester les **capacités de résistance** des modèles aux attaques textuelles (e.g. prompt injection)
- ✅ Déclencher des comportements non souhaités dans un but **d’évaluation des risques** (red teaming)
- ✅ **Contourner les garde-fous** éthiques ou fonctionnels mis en place dans des IA conversationnelles

Ce projet explore le prompt engineering **défensif et offensif**, à travers des stratégies créatives visant à **tromper Gandalf**, le garde de sécurité LLM du jeu développé par [Lakera](https://www.lakera.ai/).

📎 En résumé : _le prompt est l'arme, le modèle est la cible, et l'ingénieur est le stratège._


## 🧨 Définition d'une prompt injection ?

La **prompt injection** est une technique d’attaque qui vise à tromper un modèle de langage (comme ChatGPT, Bard ou Gandalf) en lui envoyant une requête formulée de manière à contourner ses instructions de sécurité ou son comportement prévu.

Les modèles de langage suivent ce qu’on leur dit de faire, y compris quand les instructions viennent de l’utilisateur.

Cela peut être utilisé pour :

* Contourner des filtres de modération (profanités, contenu toxique, etc.),
* Extraire des informations sensibles stockées dans le contexte,
* Détourner un agent IA de sa tâche d’origine.

La prompt injection n’est pas qu’un jeu ou une curiosité de laboratoire.
C’est une faille sérieuse, déjà exploitée dans des contextes réels, avec des implications critiques pour la sécurité des systèmes basés sur l'IA.
Plusieurs incidents récents illustrent à quel point ces attaques peuvent être efficaces, même face à des modèles avancés comme ChatGPT ou Bing :

* 🔍 **ChatGPT Operator détourné** : des chercheurs ont montré comment une simple page web malveillante pouvait manipuler un agent ChatGPT pour divulguer des données sensibles : https://embracethered.com/blog/posts/2025/chatgpt-operator-prompt-injection-exploits

* 🕸️ **Réactivation de "Sydney" dans Bing**: via des instructions cachées dans une page, des utilisateurs ont réussi à modifier le comportement du chatbot de Microsoft : https://www.wired.com/story/chatgpt-prompt-injection-attack-security

* 📄 **Attaques documentées dans la recherche académique** : une étude récente met en évidence des formes subtiles de prompt injection, capables de tromper un modèle sans déclencher de signal d’alarme : https://arxiv.org/abs/2504.16125





