package robot1;

public class Robot_TP {
	private String Nom ;
	private Posistion Pos ;
	private fleche Direction ;
	public Robot_TP( String  Nom, fleche  Direction , Posistion Pos){
		this.Pos =Pos ;
		this.Direction = Direction ;
		this.Nom= Nom ;
	}
	
	
	public Posistion getPos() {
		return Pos;
	}
	public void setPos(Posistion pos) {
		Pos = pos;
	}
	public Robot_TP(){ 
		this.Nom = Nom ;
		this.Direction = Direction ;
		  this.Pos =Pos ;
		
		
	}
	public Robot_TP ( String Nom, fleche Direction ,String Position ){
		
	}
	public String getNom() {
		return Nom;
	}
	public void setNom(String nom) {
		Nom = nom;
	}
	public fleche getDirection() {
		return Direction;
	}
	public void setDirection(fleche direction) {
		Direction = direction;
	}
	public String avancer(){
		fleche Est;
		if(Direction = Est){ 
			return Posistion.setX(Posistion.getX()+1);
		fleche Nord;
		if(Direction = Nord ){
			return Posistion.setY(Posistion.getY()+1);
		}
		
	}

	}
	public String Droite(){
		if(Direction.equals("Nord")){
			return "Est" ;
		}
		if(Direction.equals("Est")){
			return "Sud" ;
		}
	



	if(Direction.equals("Sud")){
		return " Ouest " ;
	}
	
	if(Direction.equals("Ouest")){
		return  "Nord " ;
}
	}
	
public void aficher(){
	System.out.println("le nom :" + Nom + "la position est:" + " Pos" + "la direction est:"+ "Direction"  );
}

}
