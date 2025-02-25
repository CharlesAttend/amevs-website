<script>
  import MemberCard from '$lib/component/Member_Card.svelte';
</script>

<div class="bg-base-200 hero min-h-screen">
  <div class="hero-content flex-col lg:flex-row">
    <div>
      <h1 class="text-5xl font-bold">Membres de l'association</h1>
      <!-- <button>Vois tous nos projets</button> -->
    </div>
    <div class="grid grid-rows-4 gap-4">
      <MemberCard
        name="Jéricho Pierre-Noël"
        role="Président"
        status="Étudiant en informatique"
        pp="https://media.licdn.com/dms/image/v2/D4E03AQES7M-hrCz7Qw/profile-displayphoto-shrink_800_800/profile-displayphoto-shrink_800_800/0/1684374597327?e=1746057600&v=beta&t=hfmEh6VY06m2eSzFsmUC_RyWjhhoCQ9I6g264sQ0-so"
      />
      <MemberCard
        name="Sohann"
        role="Responsable communiquation"
        status="Étudiante"
        pp="https://media-cdg4-1.cdn.whatsapp.net/v/t61.24694-24/413127217_391166153360852_5362753401083869385_n.jpg?ccb=11-4&oh=01_Q5AaIKJzWH5O6hSrSi9A9iNejAis3ImjGa6aWdplKnfH-kTY&oe=67CAB2AB&_nc_sid=5e03e0&_nc_cat=102"
      />
      <MemberCard
        name="Mélissa"
        role="Trésorière"
        status="Étudiante"
        pp="https://media-cdg4-3.cdn.whatsapp.net/v/t61.24694-24/471312336_1309053043773352_2365337457554165726_n.jpg?ccb=11-4&oh=01_Q5AaIM5Z_lAU3v-qINH-cOv6M7a1_Xn-ItGSGX21LHogDuBI&oe=67CABBAF&_nc_sid=5e03e0&_nc_cat=103"
      />
      <MemberCard
        name="Cécilia"
        role="Responsable des partenariats"
        status="Étudiante en langues étrangère"
        pp="https://media.licdn.com/dms/image/v2/D4E03AQEFvUHhIiNyxw/profile-displayphoto-shrink_800_800/profile-displayphoto-shrink_800_800/0/1730800820307?e=1746057600&v=beta&t=Q6W3rlK784SfuWYbfOen_a2pSQJFmdSQqsRAAB2oGak"
      />
    </div>
    <button class="btn btn-primary">Voir tous les membres</button>
  </div>
</div>
