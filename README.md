# contao-masonry-gallery
Contao Galerie als Masonry Galerie mit masonry.desandro.com  

[Masonry - Cascading grid layout library](https://masonry.desandro.com/)  
[imagesLoaded](https://imagesloaded.desandro.com)  

## Twig Template anpassen  
Ersetze das Core Template mit dem angepassten Template.  
Der `<ul>` wird eine Klasse `grid` hinzugefügt.  
Der `<li>` wird eine Klasse `grid-item` hinzugefügt.  

Die notwendigen JS Dateien `masonry.pkgd.min.js` und `imagesloaded.pkgd.min.js` werden direkt aus dem Template in den `body` geladen.  
Mit `{% add 'masonry_scripts' to body %}` werden die Dateien nur einmal pro Seite, und nur dort, wo das angepasste Template im Einsatz ist, geladen. Auch bei Mehrfachverwendung von Inhaltselementen Galerie mit diesem Template, werden die Dateien nur einmal geladen.  

## (S)CSS  
Mit dabei ist ein Beispiel SCSS, welches die Auswahl im Backend `Vorschaubilder pro Reihe` bis zu einer Anzahl von 6 Bilder pro Reihe, berücksichtigt.
