package Robot;

{
 private String nom;
 private int x;
 private int y;
 private String direction;

 public Robot(String nom)
 {
 this.nom = nom;
 x = y = 0;
 direction = "Est";
 }
 public Robot(String nom, int x, int y, String direction)
 {
 this(nom);
 this.x = x;
 this.y = y;
 if (direction.equals("Nord") || direction.equals("Sud")
 || direction.equals("Ouest"))
 this.direction = direction; // garder "Est" si direction invalide
 }
 /**
 * avance d'un pas
 */
 public void avance()
 {
 if (direction.equals("Nord"))
 y++;
 else if (direction.equals("Est"))
 x++;
 else if (direction.equals("Sud"))
 y--;
 else // (direction.equals("Ouest"))
 x--;
 }
 /**
 * tourne à droite de 90°
 */
 public void droite()
 {
 if (direction.equals("Nord"))
 direction = "Est";
 else if (direction.equals("Est"))
 direction = "Sud";
 else if (direction.equals("Sud"))
 direction = "Ouest";
 else // (direction.equals("Ouest"))
 direction = "Nord";
 }
 /**
 * affiche l'état du robot
 */
 public void afficher()
 {
 System.out.println("nom : " + nom);
 System.out.println("position : (" + x + "," + y +")");
 System.out.println("direction : " + direction);
 }
}
