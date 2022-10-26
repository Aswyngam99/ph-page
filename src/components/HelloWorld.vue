<template>
  <v-app>
    <v-app-bar :color="color" app dark>
      <v-img class="mx-10" src='../../public/logo.png' contain max-height="70" max-width="70"></v-img>
      <v-toolbar-title> Henkel REGHAIA </v-toolbar-title>
      <v-spacer></v-spacer>
      <span><strong>MOP-QC-DST A.1.00 / </strong>  Révision : <strong>00</strong> / Date : <strong>20.02.2022</strong></span>
    </v-app-bar>
      <v-container fluid>  
        <v-row class="align-center">
          <!-- <v-img src='../../public/labo3.jpg'></v-img> -->
          <v-col class="align-center">
          <v-row justify="center">
          </v-row>
               <v-card  tile class="hierarchy2 elevation-6 mt-4 d-flex flex-column">
                <v-card-text>
                <h2>Test method PH</h2>
                <h3>Système de Management Intégré</h3>
               </v-card-text>
         </v-card>
          <v-btn class="ma-8 align-center" outlined :color="color" @click="active = !active, ChangeTitle()">{{this.text}}</v-btn>
        <v-card tile flat class="mx-6 my-6">
         <h2 class="titre">1. Objet</h2>
            <p>Cette méthode décrit la détermination du pH de solutions et suspensions aqueuses à différentes concentrations et températures.</p>
         <h2 class="titre">2.	Domaine d'application </h2>
          <p>Cette procédure s’applique au laboratoire Henkel Reghaia pour chaque étape de préparation, avant de libérer le Bach semi fini et chaque 2h sur les lignes de production.</p>
        <h2 class="titre">3. Document de Référence</h2>
         <v-list-item two-line>
            <v-list-item-content>
                <v-list-item-title><strong>- ISO 9000 :</strong></v-list-item-title>
                <v-list-item-subtitle>Systèmes de management de la qualité — Principes essentiels et vocabulaire.</v-list-item-subtitle>
                <v-list-item-title><strong>- ISO 9001 :</strong></v-list-item-title>
                <v-list-item-subtitle>Systèmes de management de la qualité — Exigences.</v-list-item-subtitle>
                <v-list-item-title><strong>- ISO 9002 :</strong></v-list-item-title>
                <v-list-item-subtitle>Systèmes de management de la qualité — Lignes directrices pour l’application de l’ISO 9001:2015.</v-list-item-subtitle>
            </v-list-item-content>
        </v-list-item>
        <h2 class="titre">4. Définitions et Abréviations</h2>
            <p>Non indiquées.</p>
        <h2 class="titre">5. Responsabilités et Autorités</h2>
        <p>Le technicien contrôle qualité est responsable sur l’analyse. <br> Le responsable laboratoire est responsable sur la validation des méthodes.</p>
        <h2 class="titre">6. Processus</h2>
         <v-list-item two-line>
                <v-list-item-content>
                    <v-list-item-title><strong>1- Aperçu de la méthode</strong></v-list-item-title>
                    <v-list-item-subtitle>La valeur du pH est mesurée au moyen d'une électrode en verre et d'un voltmètre/pH-mètre à haute résistance.</v-list-item-subtitle>

                    <v-list-item-title><strong>2- Réactifs</strong></v-list-item-title>
                    <v-list-item-subtitle>• Eau déminéralisée ou autre solvant aqueux approprié.</v-list-item-subtitle>
                    <v-list-item-subtitle>• Solutions tampons pour l'étalonnage :</v-list-item-subtitle>
                    <v-list-item-subtitle>pH 2,00 (par ex. Riedel de Haën, article n° 38741).</v-list-item-subtitle>
                    <v-list-item-subtitle>pH 4,62 (par ex. Riedel de Haën, article n° 36050).</v-list-item-subtitle>
                    <v-list-item-subtitle>pH 7,00 (par ex. Riedel de Haën, article n° 33546).</v-list-item-subtitle>
                    <v-list-item-subtitle>pH 9,00 (par ex. Riedel de Haën, article n° 33548).</v-list-item-subtitle>
                    <v-list-item-subtitle>pH 10,00 (par ex. Riedel de Haën, article n° 33549).</v-list-item-subtitle>

                    <v-list-item-title><strong>3- Appareil</strong></v-list-item-title>
                    <v-list-item-subtitle>• Électrode monotige pour pH-mètre (ex. Schott).</v-list-item-subtitle>
                    <v-list-item-subtitle>• pH-mètre (par exemple modèle 632 ou 691, Metrohm).</v-list-item-subtitle>
                    <v-list-item-subtitle>• Agitateur/réchauffeur magnétique.</v-list-item-subtitle>
                    <v-list-item-subtitle>• Matériel de laboratoire usuel.</v-list-item-subtitle>

                    <v-list-item-title><strong>4- Procédure</strong></v-list-item-title>
                    <v-list-item-subtitle><strong>- Étalonnage du pH-mètre et de l'électrode monotige</strong></v-list-item-subtitle>
                    <v-list-item-subtitle>Le pH-mètre et l'électrode sont calibrés au moyen de solutions tampons. Le pH des solutions tampons à utiliser pour l'étalonnage doit se situer dans la plage de mesure. <br> <strong>Remarque :</strong>  Normalement, deux solutions tampons doivent être utilisées pour l'étalonnage.</v-list-item-subtitle>
                    <v-list-item-subtitle><strong>- Contrôle de l'eau déminéralisée</strong></v-list-item-subtitle>
                    <v-list-item-subtitle>Avant la mesure, l'électrode est soigneusement rincée à l'eau afin d'éviter tout transfert de solution d'échantillon ou de solution tampon. La valeur du pH de l'eau doit être de 7,0 ± 0,5 dans le cas où le pH de la substance à examiner devrait être compris entre 6 et 8.</v-list-item-subtitle>
                    <v-list-item-subtitle><strong>- Préparation des échantillons et mesure du pH</strong></v-list-item-subtitle>
                    <v-list-item-subtitle>Une quantité exacte de l'échantillon est pesée dans un bécher et dissoute/suspendue (si nécessaire) et remplie avec le solvant à la concentration souhaitée. Le mélange est agité sur un agitateur magnétique et la température de la solution d'échantillon est surveillée et ajustée, si nécessaire, au moyen d'un réchauffeur. L'échantillon doit être complètement dissous ou soigneusement mélangé. <br> Ensuite, l'agitateur est arrêté et l'électrode à tige unique est immergée dans la solution de sorte que la membrane de verre et le diaphragme soient complètement submergés. Le pH est lu après l'arrêt de l'affichage. <br> <strong> Remarque :</strong> Sachez que l'ébullition ou le chauffage de la solution d'échantillon peut altérer le résultat.</v-list-item-subtitle>
                    <v-list-item-subtitle><strong>- Résultats</strong></v-list-item-subtitle>
                    <v-list-item-subtitle>Le résultat est donné avec une décimale et indique la concentration, le solvant et la température de la solution ainsi que « selon la méthode Q-W-0013.0 ».</v-list-item-subtitle>
                    <v-list-item-subtitle><strong>- Précision</strong></v-list-item-subtitle>
                    <v-list-item-subtitle>En général, la précision de la mesure du pH peut être supposée être ±0,2 unités.</v-list-item-subtitle>
                </v-list-item-content>
            </v-list-item>
                <h2 class="titre">7. Annexes</h2>
            <v-card>
                 <v-simple-table>
                    <template v-slot:default>
                        <thead>
                            <tr>
                                <th class="text-left white--text tab"> Enregistrement </th>
                                <th class="text-left white--text tab"> Code </th>
                                <th class="text-left white--text tab"> Localisation </th>
                                <th class="text-left white--text tab"> Support </th>
                                <th class="text-left white--text tab"> Durée de conservation </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr v-for="item in things" :key="item.Enregistrement">
                                <td>{{ item.Enregistrement }}</td>
                                <td>{{ item.Code }}</td>
                                <td>{{ item.Localisation }}</td>
                                <td>{{ item.Support }}</td>
                                <td>{{ item.Durée}}</td>
                            </tr>
                        </tbody>
                    </template>
                </v-simple-table>
            </v-card>
        </v-card>
        <v-card tile class="hierarchy2 elevation-6 mt-4 d-flex flex-column jaune">
              <v-card-text>
                <strong>PR SHEQ VR A.5-01– Procédure de Veille Réglementaire</strong> <br> <div class="red--text"> Propriété exclusive de HENKEL Algérie Unité de Production Réghaia. <br> Toute reproduction intégrale ou partielle ainsi que son utilisation par, ou la communication à, des tiers, sans accord préalable écrit de l’auteur est illicite.</div> Le R-SMI est responsable de la gestion et l’application de cette procédure.
              </v-card-text>
             </v-card>
        </v-col>
          </v-row>
        
      </v-container>

    <v-bottom-navigation v-model="value" app :background-color="color" dark :input-value="active">
      <v-btn value="1" height="100%" width="100%" :color="color">
        <span>Objet</span>
        <v-icon>mdi-bookmark-outline</v-icon>
      </v-btn>
      <v-btn value="2" height="100%" width="100%" :color="color">
        <span>Domaine d’application </span>
        <v-icon>mdi-bookmark-outline</v-icon>
      </v-btn>
      <v-btn value="3" height="100%" width="100%" :color="color">
        <span>Document de Référence </span>
        <v-icon>mdi-bookmark-outline</v-icon>
      </v-btn>
      <v-btn value="4" height="100%" width="100%" :color="color">
        <span>Définitions et Abréviations </span>
        <v-icon>mdi-bookmark-outline</v-icon>
      </v-btn>
      <v-btn value="5" height="100%" width="100%" :color="color">
        <span>Responsabilités/Autorités </span>
        <v-icon>mdi-bookmark-outline</v-icon>
      </v-btn>
      <v-btn value="6" height="100%" width="100%" :color="color">
        <span>Processus </span>
        <v-icon>mdi-bookmark-outline</v-icon>
      </v-btn>
      <v-btn value="7" height="100%" width="100%" :color="color">
        <span>Annexes </span>
        <v-icon>mdi-bookmark-outline</v-icon>
      </v-btn>
      
    </v-bottom-navigation>
  </v-app>
</template>

<script>
export default {
  name: 'App',
  data: () => ({
    color: "#ff0011",
    active: true,
    text: "cacher le menu",
     things: [
          {
            Enregistrement: 'Fiche de suivi incident qualité',
            Code: 'SD SHEQ TNC 4.3.12-10',
            Localisation: 'R-SMI SharePoint /REG SMI',
            Support: 'Fichier électronique',
            Durée: '03 ans'
          },
          {
            Enregistrement: ' ',
            Code: ' ',
            Localisation: 'R-SMI SharePoint /REG SMI',
            Support: 'Fichier électronique',
            Durée: '03 ans'
          },
          {
            Enregistrement: ' ',
            Code: ' ',
            Localisation: 'R-SMI SharePoint /REG SMI',
            Support: 'Fichier électronique',
            Durée: '03 ans'
          },
          {
            Enregistrement: ' ',
            Code: ' ',
            Localisation: 'R-SMI SharePoint /REG SMI',
            Support: 'Fichier électronique',
            Durée: '03 ans'
          },
          {
            Enregistrement: ' ',
            Code: ' ',
            Localisation: 'R-SMI SharePoint /REG SMI',
            Support: 'Fichier électronique',
            Durée: '03 ans'
          },
          {
            Enregistrement: ' ',
            Code: ' ',
            Localisation: 'R-SMI SharePoint /REG SMI',
            Support: 'Fichier électronique',
            Durée: '03 ans'
          },
          {
            Enregistrement: ' ',
            Code: ' ',
            Localisation: 'R-SMI SharePoint /REG SMI',
            Support: 'Fichier électronique',
            Durée: '03 ans'
          }
        ]
    
  }),
  methods: {
    ChangeTitle(){
      if(this.text == "cacher le menu"){
        console.log("dkhelt fel if");
        this.text = "afficher le menu";
      }else{
        this.text = "cacher le menu";
      }
    }
  }
};
</script>

<style scoped>
.background {
  background-color: #f5eb7d;
}
.titre{
  color: #ff0011;
}
.tab{
  background-color: #fa3722;
}
</style>