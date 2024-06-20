# Part0-exercice-0.4

Le navigateur Chrome envoie une requête POST au serveur pour une nouvelle note, le serveur répond avec une redirection HTTP 302, demandant au navigateur de faire une nouvelle requête GET.
Le navigateur Chrome fait alors une nouvelle requête GET au serveur à la page que https://studies.cs.helsinki.fi/exampleapp/notes pour récupérer la nouvelle page de notes.
Le serveur va donc envoyer le document HTML correspondant à cette nouvelle page note, puis le navigateur va faire plusieurs requêtes GET supplémentaires pour récupérer les ressources nécessaires à l'affichage de la page, comme le fichier CSS main.css, le fichier JavaScript main.js et le fichier de données JSON data.json.
Le serveur répond à chacune de ces requêtes en envoyant les fichiers correspondants au navigateur. 
Soit une sorte de ping pong entre les 2 pour avoir l'ajout de la note sur le navigateur.
![exo0 4](https://github.com/Tokyo-Takeshi/Part0-exercice/assets/173046968/d62679c3-b8dd-45f2-9585-554177da3464)


# Part0-exercice-0.5
Le systéme de réponse reste le même sauf pour la balise de la requête au serveur qui est différente comparé au 1er exercice dans la balise Html
le fichier JSON ne propose plus de recharger l'intégralité des fichiers lorsque l'utilisateur effectue une reqête dans le formulaire. ( voir exercie 0.6 )

![mermaid-diagram-2024-06-20-162933](https://github.com/Tokyo-Takeshi/Part0-exercice-0.4/assets/173046968/e19aca09-4f21-48e3-8531-1add37c85482)

# Part0-exercice-0.6

Quand l'utilisateur entre dans le formulaire sa nouvelle note , le serveur qui reçoit la requête en HTTP POST va créer un fichier new_note_spa.JSON 
qui va être renvoyé au navigateur "chrome " ce qui va permettre à chrome de mettre à jour la page sans avoir à renvoyer d'autre requête pour recharger tout les fichiers ( main.css,spa.js, spa html ) . Plus rapide et plus efficace 
 ![new spa](https://github.com/Tokyo-Takeshi/Part0-exercice/assets/173046968/7f51b2e2-1938-4ca9-bff9-0ea4a6b9d7d5)
