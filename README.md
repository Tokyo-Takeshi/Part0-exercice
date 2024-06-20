# Part0-exercice-0.4

https://www.mermaidchart.com/app/projects/2a1804f5-42ed-483b-9327-62114e393aa1/diagrams/b201ded4-371b-45ee-9cb0-0f0cc32abcd7/version/v0.1/edit
sequenceDiagram
   chrome->>+serveur: POST https://studies.cs.helsinki.fi/exampleapp/new_notes
   serveur-->>chrome: demande de recharge la page Note Http 302,demande de requete HTTP GET
   chrome->>+serveur: GET https://studies.cs.helsinki.fi/exampleapp/notes
   serveur-->>-chrome: document HTML de la nouvelle page NOTE
   chrome->>+serveur: recharge:  GET https://studies.cs.helsinki.fi/exampleapp/main.css
    serveur-->>-chrome: ccs file
   chrome-->>serveur: recharge GET https://studies.cs.helsinki.fi/exampleapp/main.js
   serveur-->>chrome: main.js file
    chrome-->>serveur: recharge GET https://studies.cs.helsinki.fi/exampleapp/data.json
   serveur-->>chrome: data.json file

# Part0-exercice-0.5
Le systéme de réponse reste le même sauf pour la balise de la requête au serveur qui est différente comparé au 1er exercice dans la balise Html
le fichier JSON ne propose plus de recharger l'intégralité des fichiers lorsque l'utilisateur effectue une reqête dans le formulaire. ( voir exercie 0.6 )

![mermaid-diagram-2024-06-20-162933](https://github.com/Tokyo-Takeshi/Part0-exercice-0.4/assets/173046968/e19aca09-4f21-48e3-8531-1add37c85482)

# Part0-exercice-0.6
