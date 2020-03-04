1°) Cette classe ne respecte pas SRP car on remarque que l'on a 2 responsabilités dans le meme module


2°) Si la méthode de calcul change, il faut recompliler tous les programmes qui utilisent ce module meme s'ils ne n'ont aucun rapport avec la méthode calcul salaire.


3°) Si on change l'affichage par un stockage dans un fichier csv, cela règle le problème de DIP.


4°) Créons classes et attribuons à chacune une seule responsabilité:

* La classe abstraite Allemploye dediée au calcul du salaire des employers.
	
		public abstract class Allemploye{
			public double salaire();
			private String name
			public void calculSalaire(){}
		}
		
		

* La classe employe qui sera dediée à l'affichage

		Class employe2{
			private String name
			public void Affichage(){}
		}
			
	
