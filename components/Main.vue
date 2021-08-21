<!-- Please remove this file from your project -->
<template>
  <div>
    <b-card
      img-src="/logo.png"
      img-alt="logo"
      img-top
      tag="logo"
      class="mb-2"
    >
      <b-card-text class="text-center">
        <h1>L'asso d'evenementiel catho</h1>

        <b-link href="https://www.facebook.com/Thenewgenerationfrance" target="_blank" variant="primary" class="text-center">
          <b-icon-facebook></b-icon-facebook>
        </b-link>
        <b-link href="https://www.instagram.com/the_new_generation_france/" target="_blank" variant="primary" class="text-center">
          <b-icon-instagram></b-icon-instagram>
        </b-link>
      </b-card-text>
    </b-card>
    <b-row class="text-center">
      <b-col>
        Notre projet
      </b-col>
      <b-col>
        Nos events
      </b-col>
      <b-col>
        Notre équipe
      </b-col>
    </b-row>
    <b-card>
      <b-card-text class="text-center">
        <h1>Notre projet</h1>
        <p>
          The New Generation est une association d’événementiel catholique et culturel crée en février 2019 par deux amis parisiens. Le but de l’association est de proposer des événements variés (des conférences, des visites d’église, des ciné-débats, des lives thématiques ou encore des jeux de piste) tout au long de l’année aux jeunes cathos de 18-30 ans.
        </p>
        <p>
          L’activité se déroule uniquement sur Paris pour l’instant…
        </p>
      </b-card-text>
    </b-card>
    <b-card class="text-center" style="max-heigth: 2rem;">
      <h2>Nos events</h2>
      <b-carousel
        title="Nos events"
        id="carousel-1"
        v-model="slide"
        img-width="1024"
        img-height="480"
        controls
        indicators
        background="#ababab"
        style="text-shadow: 1px 1px 2px #333;"
        @sliding-start="onSlideStart"
        @sliding-end="onSlideEnd"
      >
        <b-carousel-slide
          caption="Les conférences"
          text="Nous organisons 1 à 2 conférences par an en accueillant des personnalités du monde catholique (Monseigneur de Romanet, Etienne de Montety, Antoine de Lochner…) et en traitant de sujets sérieux et contemporains (l’Engagement, la place de la religion dans le monde pro, la pornographie…)."
          img-src="/conference.jpg"
        >
        </b-carousel-slide>

        <b-carousel-slide
          caption="Les visites d'églises"
          text="Environ une fois par mois, nous organisons une visite guidée d’église parisienne suivie d’un verre dans un bar à proximité. De quoi associer culture et convivialité."
          img-src="/eglise.jpg"
        >
        </b-carousel-slide>

        <b-carousel-slide
          caption="Les ciné-débats"
          text="En physique ou en distanciel, nous visionnons des films poignants (Tu ne tueras point, Dieu n’est pas mort…) pour en débattre ensuite avec un prêtre ou entre nous."
          img-src="/cine_debat.png"
        >
        </b-carousel-slide>

        <b-carousel-slide
          caption="Les lives thématiques"
          text="Dans ce format, les abonnés deviennent acteurs de l’évènement. C’est vous qui venez témoigner d’un sujet de votre choix en live sur Facebook aux côtés d’un animateur TNG qui vous guide dans la démarche. Nombreux déjà sont venus partager seul ou à deux leur expérience sur le mariage, les fiançailles, la conversion, la route de Compostelle ou encore les missions humanitaires. Soyez le prochain !"
          img-src="/live_thematiques.png"
        >
        </b-carousel-slide>

        <b-carousel-slide
          caption="Les jeux de pistes"
          text="Souvent associés à l’événement de fin d’année, les jeux piste thématiques TNG rencontrent un franc succès. Nous vous organisons, dans Paris, des parcours semés d’énigmes et d’épreuves à résoudre en équipe dans un temps imparti. Récompense à la clé pour l’équipe gagnante !"
          img-src="/jeux_de_pistes.jpg"
        >
        </b-carousel-slide>

        <b-carousel-slide
          caption="Les dégustations"
          text="NOUVEAUTÉ : Après son succès, la dégustation « Le Vin dans la Bible » qui associait l’Histoire du vin dans la Bible à une dégustation de différents vins, les dégustations se poursuivent cette année. Affaire à suivre !"
          img-src="/degustation.jpg">
        </b-carousel-slide>
      </b-carousel>
    </b-card>
    <b-card class="text-center">
      <h2>Notre équipe</h2>
      <b-row class="text-center">
        <b-col>
          <b-img width="100px" height="100px" rounded="circle" src="/priscille.png" alt="Priscille"></b-img>
          Priscille, Présidente
        </b-col>
        <b-col>
          <b-img width="100px" height="100px" rounded="circle" src="/mathilde.jpg" alt="Mathilde"></b-img>
          Mathilde
          Secrétaire Générale
        </b-col>
        <b-col>
          <b-img width="100px" height="100px" rounded="circle" src="/louise.jpg" alt="Louise"></b-img>
          Louise
          Trésorière
        </b-col>
        <b-col>
          <b-img width="100px" height="100px" rounded="circle" src="/victoire.jpg" alt="Victoire"></b-img>
          Victoire
          Pôle Event
        </b-col>
        <b-col>
          <b-img width="100px" height="100px" rounded="circle" src="/augustin.jpg" alt="Augustin"></b-img>
          Augustin
          Pôle Partenariat
        </b-col>
      </b-row>
    </b-card>
  </div>
</template>
<script>
