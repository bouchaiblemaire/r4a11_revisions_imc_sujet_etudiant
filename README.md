Jorawar DULAI

# Application pour calculer l'IMC

## C'est quoi l'indice de masse corporel IMC ?


> L'indice de masse corporelle (IMC, en anglais *Body Mass Index*, BMI) est une grandeur qui permet d'estimer la corpulence d'une personne. Elle a été inventée par *Adolphe Quetelet*, scientifique belge fondateur de la statistique moderne; cet indice est aussi appelé indice de *Quetelet*.

Cet indice se calcule en fonction de la **taille** et de la **masse**. Bien qu'il ait été conçu au départ pour les adultes de 18 à 65 ans, de nouveaux diagrammes de croissance ont vu le jour au cours des dernières décennies pour les enfants de 0 à 18 ans. Dans les deux cas, il constitue une indication et intervient dans le calcul de l'IMG. (source *Wikipedia*)

<img width="800px" height="auto" src="images/imc_courbes.png" />


## Comment se calcule l'IMC ?

L'IMC est égale à $\frac{masse}{taille*taille}$ (la taille exprimé en **mètre**).

## Travail à faire

Compléter le projet fourni en vous basant sur les fonctionnalités que vous déduirez de l'application de démonstration. Vous penserez à internationaliser l'application pour le français et l'espagnol.


**Description textuelle du \textit{déroulement type} d'une utilisation de cette application :**
1. l'utilisateur saisi son nom et son prénom,
2. l'utilisateur saisi sa date de naissance,
3. l'utilisateur saisi son poids,
4. l'utilisateur saisi sa taille en centimètres ou en mètre(s). **Il devra indiqué le mode choisi gr\^ace au bouton radio de l'interface afin que le calcul de l'IMC se fasse correctement**.
5. l'utilisateur appuie sur la touche `Calculer` , le résultat s'affiche dans une autre activité.
6. lorsque l'utilisateur appuie sur le bouton `back` de l'application (pas celle du terminal), un historique est affiché en bas de la première activité sous forme de liste (`RecyclerView`).


**De plus :**

* A tout moment l'utilisateur pourra appuyer sur le bouton `RAZ` permettant d'effacer toutes les informations déjà saisies.
* Toutes les erreurs sont indiquées par des Toasts appropriés (par exemple, demande de calcul sans avoir entré les informations nécessaires etc.)




**Avant de commencer !**

Vous disposez :

* d'une [application de démonstration](https://einfo-learning.fr/moodle/mod/resource/view.php?id=13107) sous forme d'archive APK à installer sur l'émulateur.
  Pour installer l'application sur émulateur ou terminal physique (pour simplifier un seul devra être connecté)  :
  1. Lancer l'émulateur ou connecter le terminal physique
  2. `adb devices ` : Permet d'afficher les terminaux connecté à l'ordinateur
  3. `adb install nom_archive.apk` : Installe l'application sur le terminal
* d'une documentation sur les parcelables (on vous demande de comprendre l'intérêt des parcelables et non de les développer)
* d'un **certain nombre de classes** (déjà intégrées au projet Android Studio) et qu'il ne faudra pas modifier :
  * `FicheIMC`: classe `Parcelable` (c'est à dire, dont les instances sont "transportables" par un `Intent` en tant que *données extras* peut-être utilisée pour assurer une communication à l'intérieur d'une application entre activités. 
  > Un `Intent` pourra, par exemple, transporter une instance de cette classe en tant que données extras. 

:dart: En d'autres termes, toutes ces ressources vous permettent de vous concentrer sur les notions abordées lords des cours. 

:pencil: Je vous conseille de bien étudier les sources Java et les ressources XML !

## Partie 1
**Question 1 :** Versionnage de votre développement
1. cloner le présent dépôt et vous l'approprier dans votre propre dépôt git.
2. inscrire en première ligne du fichier `README.md` votre *nom*, *prenom* et *groupe*
3. créer votre propre dépôt privée et *pusher* le projet initial en tant que branche `main`
4. inscrire votre enseignant comme participant à votre déopôt git


**Question 2 :** Traduire l'application en français et en espagnol
1. créer la branche `traduction_dev`
2. traduire votre application en français et en espagnol
3. effectuer un *pull request* (ne pas effacer cette branche après l'accepation de de la demande de *pull request*)
   

**Question 3 :** Compléter les layouts pour que les interfaces utilisateurs ressemblent à celles de l'application de démonstration.
1. créer la branche `layouts_dev`
2. développer les layouts
3. effectuer un *pull request*  (ne pas effacer cette branche après l'accepation de de la demande de *pull request*)
   

**Question 4 :** Complétez les classes Java pour permettre la saisie correcte des informations et la préparation correcte de l'intention 

**Note :** On se place juste au point qui précède de lancement de l'activité cible.

1. créer la branche `dev_input_activity`
2. développer les fonctionnalités demandées
3. utiliser le mode déboggage pour vous assurer que l'intention est *correctement péparée* 
4. effectuer un *pull request*  (ne pas effacer cette branche après l'accepation de de la demande de *pull request*)
   

   
**Question 5 :** Complétez les classes Java pour permettre le calcul de l'IMC, son affichage dans l'activité cible et la préparation de l'intention de résultat

**Note :** On se place juste au point qui précède de la *teerminaison* de l'activité cible.

1. créer la branche `dev_calcul_and_print_imc`
2. développer les fonctionnalités demandées
3. utiliser le mode déboggage pour vous assurer que l'intention de résultat est *correctement péparée* 
4. effectuer un *pull request*  (ne pas effacer cette branche après l'accepation de de la demande de *pull request*)
   

   
**Question 6 :** Finaliser le développement de votre application

**Note :** On se place juste au point qui précède de la *teerminaison* de l'activité cible.

1. créer la branche `finalise_dev`
2. développer les fonctionnalités demandées
3. utiliser le mode déboggage pour vous assurer que l'intention de résultat est *correctement péparée* 
4. effectuer un *pull request*  (ne pas effacer cette branche après l'accepation de de la demande de *pull request*)
   

## Partie 2

Nous souhaitons faire évoluer l'application pour qu'un historique soit affiché dans l'activité développée dans la branche git `dev_input_activiy` sous forme d'une `RecyclerView` à la place de la `TextView`.


## Travail à faire

Compléter le projet fourni en vous basant sur les fonctionnalités que vous déduirez de l'application de démonstration. 


**Avant de commencer !**

Vous disposez :

* d'une [application de démonstration](https://einfo-learning.fr/moodle/mod/resource/view.php?id=13131) sous forme d'archive APK à installer sur l'émulateur.
  Pour installer l'application sur émulateur ou terminal physique (pour simplifier un seul devra être connecté)  :
  1. Lancer l'émulateur ou connecter le terminal physique
  2. `adb devices ` : Permet d'afficher les terminaux connecté à l'ordinateur
  3. `adb install nom_archive.apk` : Installe l'application sur le terminal
* de supports de cours pour découvrir la `RecyclerView`
* des sources de l'application abordée dans le cours les supports de cours sous la [forme d'un dépôt git](https://github.com/bouchaiblemaire/R4A11_cours_recyclerview.git)


1. créer la branche `dev_recyclerview_feature`
2. développer les fonctionnalités demandées
3. effectuer un *pull request*  (ne pas effacer cette branche après l'accepation de de la demande de *pull request*)
   
**Quelques indications :**

### **En ce qu concerne les dépendances de Gradle:**
1. Ajouter la dépendance permettant l'utilisation du composant graphique `RecyclerView` (fichier `build.gradle`du module):
  ```xml
      implementation "com.android.support:recyclerview-v7:24.0.0"
  ```

2. Synchroniser votre gradle pour tenir compte de la modification.
   
### **En ce qui concerne les layouts :**

1. Mettre à jour le layout `activity_main.xml` pour que ce soit une `RecyclerView` qui soit utilisé 
2. Créer le layout `content_cell.xml` qui décrit une cellule (ligne) de la `RecyclerView` ; voici une ébauche à compléter :
  ```xml
<?xml version="1.0" encoding="utf-8"?>
<!--
Layout pour une ligne de la RecyclerView
-->

<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:orientation="vertical"
    android:padding="10dp"
    android:layout_margin="10dp"
    android:background="@android:color/holo_blue_light"
    >

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">

        <TextView
            android:layout_width="100dp"
            android:layout_height="wrap_content"
            android:text="@string/last_name" />

        <TextView
            android:id="@+id/tv_last_name"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
           />

    </LinearLayout>

</LinearLayout>
"
  ```

### **En ce qui concerne les classes Java :**

1. Créer une classe `recyclerview.IMCViewHolder` en partant de l'ébauche suivante  :
```java
public class IMCViewHolder extends RecyclerView.ViewHolder {

    private final TextView _tvLastName=null;
    private final TextView _tvBirthday=null;
    private final TextView _tvIMC=null;

    /**
     * Instancie un ViewHolder et le rattache à une cellule (View)
     *
     * @param cell (View) : cellule à laquelle il faut rattacher
     *             le ViewHolder
     */
    public IMCViewHolder(View cell) {
        super(cell);

        // Désérialisation des componsants graphiques d'une cellule

        // A compléter
    }

    /**
     * Méthode utilitaire qui permet de remplir les champs de la cellule
     * courante  avec les informations qui lui est destinée (issue de l'Adapter)
     *
     * @param ficheIMC (FicheIMC) : fiche IMC qui devra "remplir la cellule"
     */
    public void printFicheIMCInCell(FicheIMC ficheIMC) {
       // Met à jour la cellule de la RercyclerView avec les données issues de la ficheIMC

        // A compléter


    }
}
```

2. Créer une classe `recyclerview.AdaptarIMC` en partant de l'ébauche suivante  :
```java
public class AdapterIMC extends RecyclerView.Adapter <IMCViewHolder> {
    /**
     * Contexte de l'Activity auquel est rattaché le RecyclerView
     */
    private Context _context;

    /**
     * Représente les informations que devra visualiser
     * la ListView qui sera rattachée à l'Adapter
     */
    private ArrayList<FicheIMC> _listeFicheIMC;


    /**
     * Constructeur de l'Adapter
     *
     * @param context (Context) : Contexte de l'Activity auquel est rattaché
     *                            le RecyclerView
     * @param listeFicheIMC  (ArrayList<FicheIMC) : Liste des ficheIMC qui
     *                                       "alimenteront" le RecyclerView
     */
    public AdapterIMC(Context context, ArrayList<FicheIMC> listeFicheIMC) {
    
        
        // A compléter

        /**
         * Notifie au RecyclerView qu'il doit se rafraichir
         */
        notifyDataSetChanged();
    }

    /**
     * Permet de créer les cellules visibles
     * Est appelé une seule fois
     * @param parent (ViewGroup) : Parent auquel sera ajouté la cellule qui
     *                             va être crée
     * @param viewType
     * @return (IMCViewHolder) : Cellule qui est crée et initialisée
     */
    @Override
    public IMCViewHolder onCreateViewHolder(ViewGroup parent, int viewType) {
        /**
         * Déserialisation de la cellule
         * La valeur false permet de ne pas rattacher la cellule directement
         * au parent, mais de laisser cette responsabilité au RecyclerView
         */
        View cell = null;
               
        // A ccompléter
        
        /**
         * Remplissage de la cellule
         */
        IMCViewHolder ficheIMCViewHolder = null;
        
        // A compléter
        return ficheIMCViewHolder;
    }

    /**
     * Permet de remplir les cellules visibles
     * @param holder (ContactViewHolder) : cellule à remplir
     * @param position (int) : position de la cellule dans la liste
     */
    @Override
    public void onBindViewHolder(IMCViewHolder holder, int position) {
        
        // A compléter
    }

    /**
     * Nombre total de cellules (visibles et non visibles) du RecyclerView
     * @return (int) : Nombre total de cellules présentes dans le RecyclerView
     */
    @Override
    public int getItemCount() {
        int itemCount = 0;

        if (this._listeFicheIMC !=null){
            itemCount = this._listeFicheIMC.size();
        }
        return itemCount;
    }

    // Ajoute une ficheIMC
    public void addFicheIMC(FicheIMC ficheIMC){
        this._listeFicheIMC.add(ficheIMC);

        notifyDataSetChanged();
    }
} // Fin de la classe ContactsAdapter

```

3.  Modifier la classe `MainActivity` en appuyant de l'ébauche suivante 
```java

/**
 * Saisie des informations de l'utilisateur
 * Affichage de l'historique des informations et des IMCs calculés
 *
 * @author B. LEMAIRE
 * @version 2023
 */
public class MainActivity extends Activity {

	public static final String FICHE_IMC = "fiche_imc"; /* clef pour l'envoie de la fiche IMC en
	                                                       tant qu'extra d'un intent */

	private static final int REQ_IMC = 1;				/* Code de requête pour le résultat de
														   retour d'une activité */

	// Champs de saisis des informations
	private EditText ed_nom = null;
	private EditText ed_prenom = null;
	private EditText ed_poids = null;
	private EditText ed_taille = null;

	// Permet de saisir la date de naissance
	private DatePicker date_picker = null;

	// Groupe raido pour saisir l'unité de la taille (mètre ou centimètre)
	private RadioGroup group = null;


	// Liste des ficheIMC
	private RecyclerView _rv_ficheIMC = null;

	private AdapterIMC adapterIMC = null;


	@Override
	public void onCreate(Bundle savedInstanceState) {
		super.onCreate(savedInstanceState);
		
   // ...

		/**
		 * Instanciation de l'Adapter qui alimentera le RecyclerView
		 */

		 // A compléter

		/**
		 * Association du RecyclerView avec son Adaptateur qui l'alimentera avec
		 * les ficheIMC
		 */

		// A compléter

	}

	private void deserialiserRessource() {

	  // ...

		// Desérialisation du RecyclerView

		// A compléter
	}

  // ...

	@Override
	protected void onActivityResult(int requestCode, int resultCode, Intent data) {


		// A compléter

		super.onActivityResult(requestCode, resultCode, data);
	}

  // ...

}
```
