    Méthode pour lancer le dé, tirer un chiffre aléatoire et déplacer le personnage sur le plateau
    
     public static int nombreAleatoire() {  
        System.out.println("lancer le jeu ? \n1- oui \n2-non"); 
        int nb = sc.nextInt();  
        int cases = 0;  
        sc.nextLine();  
        int n = 0;   
        int resultat;  
        if (nb == 1) {  
            do {  
                System.out.println("Lancer le dé ? \n 1 - oui \n 2 - non");  
                resultat = sc.nextInt();  
                if (resultat == 1) {  
                    Random r = new Random(); // classe pour pouvoir utiliser le tirage aléatoire  
                        n = r.nextInt(6) + 1; //permet un tirage entre 0 et 5, on y ajoute un pour ne pas tomber sur 0 et avoir 6  
  
                    System.out.println("Vous avez fait : " + n);
                    cases = cases + n;

                    if (cases >= 64) {
                        System.out.println("Vous avez gagné!!");
                    } else {
                        System.out.println("Vous êtes à la case : " + cases);
                    }
                } else {
                    System.out.println("A bientôt");
                }
            }
            while (cases < 64 && resultat == 1);
        } else {
            System.out.println("A bientôt");
        }


        return n;
    }