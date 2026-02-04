<details class="flèche-droite">
  <summary>Voir plus</summary>
  <p>Voici le contenu caché qui apparaît quand on clique.</p>
</details>

<style>
/* Masquer la flèche par défaut */
details.flèche-droite summary {
  list-style: none;      /* supprime le triangle natif */
  display: flex;
  justify-content: space-between; /* texte à gauche, flèche à droite */
  align-items: center;
  cursor: pointer;
}

/* Créer une flèche personnalisée */
details.flèche-droite summary::after {
  content: '▶';          /* triangle pointant vers la droite */
  transition: transform 0.3s;
}

/* Rotation de la flèche quand le <details> est ouvert */
details.flèche-droite[open] summary::after {
  transform: rotate(90deg); /* pointe vers le bas */
}
</style>
