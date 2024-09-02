
<!DOCTYPE html>
<html>
    <body>
        <h1>La géolocalisation des hôtels les plus proches en Utilisant Neo4j et l'Algorithme de Dijkstra</h1>
        <p>
            Ce projet permet de localiser les hôtels les plus proches d'un point donné et de visualiser le chemin 
            le plus court pour y accéder. Le projet utilise la base de données graphe Neo4j pour stocker 
            les informations géographiques des hôtels et leurs relations, tandis que l'algorithme de Dijkstra 
            est implémenté pour calculer le chemin optimal. L'interface utilisateur affiche les résultats 
            sur une carte interactive ainsi que dans une fenêtre Tkinter, offrant une expérience utilisateur intuitive.
        </p>
        <h2>Fonctionnalités :</h2>
         <ul>
            <li>Stockage des Données : Gestion des informations des hôtels sous forme de nœuds dans Neo4j.</li>
            <li>Calcul du Chemin le Plus Court : Utilisation de l'algorithme de Dijkstra pour calculer le chemin le plus court entre un point de départ et un hôtel.</li>
            <li>Visualisation Interactive : Affichage du chemin sur une carte interactive avec des informations détaillées sur les hôtels.</li>
            <li>Interface Graphique : Une interface utilisateur intuitive qui permet de visualiser et d'explorer les hôtels les plus proches.</li>
          </ul>
        <h2>Le projet est divisé en deux parties :</h2>
        <ul><li>
        <h4>Stockage des Nœuds dans Neo4j</h4>
            <ul>
                <li>Cette section se charge de la gestion des données des hôtels, y compris leurs coordonnées géographiques et les relations entre les différents points d'intérêt.</li>
                <li>Neo4j est utilisé pour stocker les hôtels sous forme de nœuds dans une base de données graphe. Les relations entre ces nœuds (par exemple, les routes) sont également stockées pour permettre un calcul efficace du chemin.</li>
                <li>Les données sont manipulées avec des requêtes Cypher pour insérer, mettre à jour, et récupérer les informations nécessaires.</li>
            </ul>
        </li>
        <li>
        <h4>Algorithme de Dijkstra et Affichage</h4>
            <ul>
                <li>L'algorithme de Dijkstra est utilisé pour trouver le chemin le plus court entre un point de départ et les hôtels les plus proches.</li>
                <li>Le chemin est ensuite visualisé sur une carte interactive grâce à la bibliothèque Folium. Les hôtels sont représentés par des marqueurs, et les détails tels que le nom, l'adresse, et les images des hôtels sont affichés dans des pop-ups.</li>
                <li>Une interface graphique créée avec Tkinter présente des informations détaillées sur l'hôtel sélectionné, y compris l'image, les coordonnées et le chemin le plus court.</li>
            </ul>
        </li>
        </ul>
        <h2>Technologies Utilisées:</h2>
        <ul>
        <li>Neo4j
            <ul>
                <li>Description : Neo4j est une base de données orientée graphe qui permet de stocker et de requêter des relations complexes entre des données géolocalisées.</li>
                <li>Utilisation : Stockage des hôtels et des relations entre eux sous forme de nœuds et d'arêtes. Les requêtes Cypher sont utilisées pour récupérer les chemins et les hôtels.</li>
            </ul>
        </li>
        <li>
        Python :
           <ul>
             <li>Description : Python est le langage principal utilisé pour le développement du projet.</li>
             <li>Utilisation : Python est utilisé pour la manipulation des données dans Neo4j, l'implémentation de l'algorithme de Dijkstra, et le développement de l'interface utilisateur.</li>
            </ul>
        </li>
        <li>
        Driver Python Neo4j (neo4j library) :
            <ul>
              <li>Description : Le driver officiel de Neo4j pour Python, permettant d’interagir avec la base de données Neo4j depuis le code Python.</li>
              <li>Utilisation : Permet la connexion à Neo4j, l'exécution de requêtes Cypher pour interagir avec les nœuds et les relations stockés.</li>
            </ul>
        </li>
        <li>
        Folium :
            <ul>
              <li>Description : Folium est une bibliothèque Python qui permet de créer des cartes interactives avec Leaflet.js.</li>
              <li>Utilisation : Visualisation du chemin le plus court sur une carte interactive, avec des marqueurs pour les hôtels et des informations affichées dans des pop-ups.</li>
            </ul>
        </li>
        <li>
        Tkinter :
            <ul>
              <li>Description : Tkinter est la bibliothèque graphique standard pour Python.</li>
              <li>Utilisation : Création de l'interface utilisateur pour afficher les informations détaillées sur les hôtels, y compris une carte interactive intégrée.</li>
            </ul>
        </li>
        <li>
        TkinterMapView :
            <ul>
              <li>Description : Un widget Tkinter permettant d'afficher des cartes interactives.</li>
              <li>Utilisation : Intégration d'une carte interactive dans l'interface Tkinter pour visualiser le chemin vers les hôtels à partir de l'application.</li>
            </ul>
        </li>
        <li>
        Pillow (PIL) :
            <ul>
              <li>Description : Pillow est une bibliothèque d'imagerie pour Python.</li>
              <li>Utilisation : Chargement et affichage des images des hôtels dans l'interface Tkinter.</li>
            </ul>
        </li>
        <li>
        Requests :
            <ul>
              <li>Description : Une bibliothèque Python utilisée pour effectuer des requêtes HTTP.</li>
              <li>Utilisation : Récupération d'images des hôtels à partir d'URLs et affichage dans l'application.</li>
            </ul>
        </li>
        </ul>
    </body>
</html>
