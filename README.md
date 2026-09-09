<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <meta name="description" content="Portfolio personal Jihan Maharani Putri">
  <meta name="author" content="Jihan Maharani Putri">

  <title>Jihan Maharani Putri | Personal Portfolio</title>

  <script src="https://cdn.tailwindcss.com"></script>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Pacifico&display=swap" rel="stylesheet">

  <link rel="stylesheet"
        href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

  <style>
    :root{
      --pink:#f472b6;
      --pink-dark:#db2777;
      --pink-soft:#fce7f3;
      --cream:#fffaf5;
      --text:#4a3040;
    }

    *{
      box-sizing:border-box;
      scroll-behavior:smooth;
    }

    body{
      margin:0;
      color:var(--text);
      font-family:"DM Sans",sans-serif;
      overflow-x:hidden;

      background:
        radial-gradient(
          circle at 8% 8%,
          rgba(244,114,182,.15),
          transparent 24%
        ),
        radial-gradient(
          circle at 92% 20%,
          rgba(251,207,232,.35),
          transparent 25%
        ),
        var(--cream);
    }

    .cute-font{
      font-family:"Pacifico",cursive;
    }

    .cute-card{
      background:rgba(255,255,255,.82);
      border:1px solid rgba(244,114,182,.18);
      box-shadow:0 15px 45px rgba(219,39,119,.08);
      backdrop-filter:blur(12px);
      transition:.3s;
    }

    .cute-card:hover{
      transform:translateY(-5px);
      box-shadow:0 20px 50px rgba(219,39,119,.14);
    }

    .pink-btn{
      background:linear-gradient(
        135deg,
        #f472b6,
        #ec4899
      );
      color:#fff;
      transition:.3s;
      box-shadow:0 8px 25px rgba(236,72,153,.22);
    }

    .pink-btn:hover{
      transform:translateY(-3px);
      box-shadow:0 12px 30px rgba(236,72,153,.35);
    }

    .outline-btn{
      border:1.5px solid #f472b6;
      color:#db2777;
      transition:.3s;
    }

    .outline-btn:hover{
      background:#fce7f3;
      transform:translateY(-3px);
    }

    .nav-link{
      position:relative;
      transition:.25s;
    }

    .nav-link:hover{
      color:#db2777;
    }

    .nav-link::after{
      content:"";
      position:absolute;
      width:0;
      height:2px;
      bottom:-5px;
      left:50%;
      background:#ec4899;
      transition:.3s;
      transform:translateX(-50%);
    }

    .nav-link:hover::after{
      width:70%;
    }

    .photo-placeholder{
      background:linear-gradient(
        135deg,
        #fce7f3,
        #fff1f2
      );
      border:2px dashed rgba(236,72,153,.35);
      color:#db2777;
    }

    .gallery-img{
      transition:.4s;
    }

    .gallery-item:hover .gallery-img{
      transform:scale(1.06);
    }

    .float{
      animation:float 4s ease-in-out infinite;
    }

    @keyframes float{
      0%,100%{
        transform:translateY(0);
      }

      50%{
        transform:translateY(-12px);
      }
    }

    .sparkle{
      position:fixed;
      z-index:9999;
      pointer-events:none;
      color:rgba(236,72,153,.55);
      animation:sparkle 3s ease-in-out infinite;
    }

    @keyframes sparkle{
      0%,100%{
        opacity:.15;
        transform:scale(.7) rotate(0);
      }

      50%{
        opacity:1;
        transform:scale(1.3) rotate(180deg);
      }
    }

    .reveal{
      opacity:0;
      transform:translateY(35px);
      transition:.8s;
    }

    .reveal.active{
      opacity:1;
      transform:translateY(0);
    }

    #mobileMenu{
      display:none;
    }

    #mobileMenu.show{
      display:block;
    }

    .timeline-line{
      position:absolute;
      left:16px;
      top:0;
      bottom:0;
      width:2px;
      background:
        linear-gradient(
          #f9a8d4,
          #f472b6,
          #fbcfe8
        );
    }

    .music-player{
      position:fixed;
      right:20px;
      bottom:20px;
      z-index:1000;
    }

    #galleryModal{
      background:rgba(42,20,32,.84);
      backdrop-filter:blur(8px);
    }

    .memory-card{
      cursor:pointer;
    }

    @media(max-width:768px){

      .hero-title{
        font-size:2.8rem;
      }

      .music-player{
        right:12px;
        bottom:12px;
      }

      section{
        scroll-margin-top:80px;
      }
    }
  </style>
</head>

<body>

  <!-- =========================
       DECORASI
  ========================== -->

  <div aria-hidden="true">

    <span class="sparkle"
          style="left:5%;top:15%">
      ✦
    </span>

    <span class="sparkle"
          style="left:15%;top:65%;animation-delay:.8s">
      ✧
    </span>

    <span class="sparkle"
          style="left:28%;top:30%;animation-delay:1.2s">
      ✦
    </span>

    <span class="sparkle"
          style="left:42%;top:80%;animation-delay:.4s">
      ✧
    </span>

    <span class="sparkle"
          style="left:58%;top:18%;animation-delay:1.5s">
      ✦
    </span>

    <span class="sparkle"
          style="left:70%;top:55%;animation-delay:.7s">
      ✧
    </span>

    <span class="sparkle"
          style="left:82%;top:25%;animation-delay:1s">
      ✦
    </span>

    <span class="sparkle"
          style="left:94%;top:75%;animation-delay:.3s">
      ✧
    </span>

  </div>


  <!-- =========================
       NAVBAR
  ========================== -->

  <header class="fixed top-0 left-0 right-0 z-50">

    <nav class="mx-auto max-w-7xl px-4 py-4">

      <div class="cute-card rounded-full px-5 py-3 flex items-center justify-between">

        <a href="#beranda"
           class="cute-font text-xl text-pink-500">
          Jihan ♡
        </a>


        <div class="hidden lg:flex items-center gap-6 text-sm font-semibold">

          <a class="nav-link" href="#beranda">
            Beranda
          </a>

          <a class="nav-link" href="#tentang">
            Tentang
          </a>

          <a class="nav-link" href="#cv">
            CV
          </a>

          <a class="nav-link" href="#foto">
            Foto
          </a>

          <a class="nav-link" href="#sosial">
            Sosial
          </a>

          <a class="nav-link" href="#kontak">
            Kontak
          </a>

          <a class="nav-link" href="#testimoni">
            Testimoni
          </a>

        </div>


        <button id="menuBtn"
                class="lg:hidden w-10 h-10 rounded-full bg-pink-100 text-pink-600"
                aria-label="Buka menu">

          <i class="fa-solid fa-bars"></i>

        </button>

      </div>


      <!-- MOBILE MENU -->

      <div id="mobileMenu"
           class="cute-card mt-2 rounded-3xl p-5 lg:hidden">

        <div class="grid grid-cols-2 gap-3 text-sm font-semibold">

          <a href="#beranda">
            Beranda
          </a>

          <a href="#tentang">
            Tentang
          </a>

          <a href="#cv">
            CV
          </a>

          <a href="#foto">
            Foto
          </a>

          <a href="#sosial">
            Sosial
          </a>

          <a href="#kontak">
            Kontak
          </a>

          <a href="#testimoni">
            Testimoni
          </a>

        </div>

      </div>

    </nav>

  </header>


  <main>

    <!-- =========================
         HERO
    ========================== -->

    <section id="beranda"
             class="min-h-screen flex items-center pt-32 pb-20 px-5">

      <div class="max-w-7xl mx-auto w-full grid lg:grid-cols-2 gap-14 items-center">

        <div class="reveal">

          <span class="inline-block px-4 py-2 rounded-full bg-pink-100 text-pink-600 text-sm font-bold mb-5">
            ✨ Welcome to my little world
          </span>


          <h1 class="hero-title text-5xl md:text-6xl font-bold leading-tight">

            Halo, aku
            <span class="text-pink-500">
              Jihan
            </span>
            🎀

          </h1>


          <p class="cute-font text-2xl text-pink-400 mt-4">
            Jihan Maharani Putri
          </p>


          <p class="mt-5 text-lg text-gray-600 max-w-xl leading-relaxed">

            Seorang
            <b>pelajar</b>
            yang aktif, berjiwa juang, tangguh,
            kreatif, dan senang mencoba hal-hal baru.

          </p>


          <div class="flex flex-wrap gap-4 mt-8">

            <a href="#foto"
               class="pink-btn px-6 py-3 rounded-full font-bold">

              📸 Lihat Memories

            </a>


            <a href="#kontak"
               class="outline-btn px-6 py-3 rounded-full font-bold">

              💌 Hubungi Saya

            </a>

          </div>


          <div class="flex gap-5 mt-8 text-pink-400 text-xl">

            <span>♡</span>
            <span>✦</span>
            <span>୨୧</span>
            <span>✧</span>
            <span>♡</span>

          </div>

        </div>


        <!-- FOTO PROFIL PALING ATAS -->

        <div class="reveal flex justify-center relative">

          <div class="absolute -top-8 -left-4 text-4xl float">
            🎀
          </div>

          <div class="absolute -bottom-5 -right-2 text-4xl float">
            ✨
          </div>

          <div class="absolute top-1/2 -right-8 text-3xl float">
            💗
          </div>


          <div class="w-72 h-72 md:w-96 md:h-96 rounded-[45%] p-3 bg-gradient-to-br from-pink-200 via-white to-pink-300 shadow-2xl">

            <div class="w-full h-full rounded-[42%] overflow-hidden photo-placeholder">

              <img src="assets/images/profile.jpg"
                   alt="Foto profil Jihan"
                   class="w-full h-full object-cover"
                   onerror="this.style.display='none';this.nextElementSibling.style.display='flex';">


              <div class="hidden w-full h-full flex-col items-center justify-center text-center p-5">

                <i class="fa-solid fa-image text-5xl mb-3"></i>

                <b>
                  Foto Profil
                </b>

                <small>
                  profile.jpg
                </small>

              </div>

            </div>

          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         ABOUT
    ========================== -->

    <section id="tentang"
             class="py-24 px-5">

      <div class="max-w-7xl mx-auto">


        <div class="text-center reveal">

          <span class="text-pink-500 font-bold">
            ♡ ABOUT ME ♡
          </span>

          <h2 class="text-4xl font-bold mt-2">
            Tentang Saya
          </h2>

          <p class="text-gray-500 mt-3">
            Sedikit cerita tentang Jihan ✨
          </p>

        </div>


        <div class="grid lg:grid-cols-2 gap-10 mt-14 items-center">


          <!-- FOTO JIHAN -->

          <div class="reveal">

            <div class="cute-card rounded-[35px] p-4">

              <div class="aspect-[4/3] rounded-[28px] overflow-hidden photo-placeholder">

                <img src="assets/images/jihan-about.jpg"
                     alt="Foto Jihan"
                     class="w-full h-full object-cover"
                     onerror="this.style.display='none';this.nextElementSibling.style.display='flex';">


                <div class="hidden w-full h-full flex-col items-center justify-center">

                  <i class="fa-solid fa-camera text-4xl mb-2"></i>

                  <span>
                    Foto Tentang Saya
                  </span>

                </div>

              </div>

            </div>

          </div>


          <!-- PENJELASAN -->

          <div class="reveal">

            <h3 class="text-3xl font-bold">

              Hai! Aku
              <span class="text-pink-500">
                Jihan
              </span>
              🎀

            </h3>


            <p class="text-gray-600 leading-relaxed mt-5">

              Aku adalah seorang pelajar yang aktif dan memiliki semangat
              untuk terus belajar serta berkembang. Aku percaya bahwa setiap
              proses memberikan pengalaman yang berharga.

            </p>


            <p class="text-gray-600 leading-relaxed mt-4">

              Aku juga memiliki jiwa juang dan tangguh dalam menghadapi
              berbagai tantangan. Bagiku, mencoba, belajar, dan terus
              berkembang adalah bagian dari perjalanan yang menyenangkan.

            </p>


            <div class="grid grid-cols-2 gap-4 mt-8">

              <div class="cute-card rounded-3xl p-5 text-center">

                <div class="text-3xl">
                  💻
                </div>

                <h4 class="font-bold mt-2">
                  Web
                </h4>

                <p class="text-sm text-gray-500">
                  Basic Web Development
                </p>

              </div>


              <div class="cute-card rounded-3xl p-5 text-center">

                <div class="text-3xl">
                  🎨
                </div>

                <h4 class="font-bold mt-2">
                  Desain
                </h4>

                <p class="text-sm text-gray-500">
                  Creative Design
                </p>

              </div>

            </div>

          </div>

        </div>


        <!-- =========================
             HOBBIES
        ========================== -->

        <div class="mt-24 reveal">

          <div class="text-center mb-10">

            <span class="text-pink-500 font-bold">
              ୨୧ MY HOBBIES ୨୧
            </span>

            <h3 class="text-3xl font-bold mt-2">
              Hal yang Aku Suka
            </h3>

            <p class="text-gray-500 mt-3">
              Klik foto untuk melihat ceritanya 💗
            </p>

          </div>


          <div class="grid md:grid-cols-3 gap-6">


            <!-- HOBI 1 -->

            <div class="cute-card rounded-3xl overflow-hidden gallery-item memory-card"
                 onclick="openInfo(
                   'Roller Skating 🛼',
                   'Suka menikmati waktu dengan bermain sepatu roda, belajar gerakan baru, dan seru-seruan sambil tetap aktif.',
                   'assets/images/hobi-1.jpg'
                 )">

              <div class="h-64 photo-placeholder overflow-hidden">

                <img src="assets/images/hobi-1.jpg"
                     alt="Roller skating"
                     class="gallery-img w-full h-full object-cover">

              </div>


              <div class="p-5">

                <h4 class="font-bold text-lg">
                  Roller Skating 🛼
                </h4>

                <p class="text-gray-500 text-sm mt-2">
                  Klik untuk lihat cerita ✨
                </p>

              </div>

            </div>


            <!-- HOBI 2 -->

            <div class="cute-card rounded-3xl overflow-hidden gallery-item memory-card"
                 onclick="openInfo(
                   'Singing 🎤',
                   'Bernyanyi jadi salah satu cara untuk menikmati musik, mengekspresikan diri, dan mengisi waktu dengan hal yang menyenangkan.',
                   'assets/images/hobi-2.jpg'
                 )">

              <div class="h-64 photo-placeholder overflow-hidden">

                <img src="assets/images/hobi-2.jpg"
                     alt="Singing"
                     class="gallery-img w-full h-full object-cover">

              </div>


              <div class="p-5">

                <h4 class="font-bold text-lg">
                  Singing 🎤
                </h4>

                <p class="text-gray-500 text-sm mt-2">
                  Klik untuk lihat cerita ✨
                </p>

              </div>

            </div>


            <!-- HOBI 3 -->

            <div class="cute-card rounded-3xl overflow-hidden gallery-item memory-card"
                 onclick="openInfo(
                   'Traditional Dance 🌺',
                   'Tertarik dengan seni tari tradisional dan keindahan gerakan yang penuh makna, sekaligus ikut mengenal budaya Indonesia.',
                   'assets/images/hobi-3.jpg'
                 )">

              <div class="h-64 photo-placeholder overflow-hidden">

                <img src="assets/images/hobi-3.jpg"
                     alt="Tari tradisional"
                     class="gallery-img w-full h-full object-cover">

              </div>


              <div class="p-5">

                <h4 class="font-bold text-lg">
                  Traditional Dance 🌺
                </h4>

                <p class="text-gray-500 text-sm mt-2">
                  Klik untuk lihat cerita ✨
                </p>

              </div>

            </div>

          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         CV
    ========================== -->

    <section id="cv"
             class="py-24 px-5 bg-white/50">

      <div class="max-w-5xl mx-auto">


        <div class="text-center reveal">

          <span class="text-pink-500 font-bold">
            ✦ MY JOURNEY ✦
          </span>

          <h2 class="text-4xl font-bold mt-2">
            Curriculum Vitae
          </h2>

        </div>


        <div class="relative mt-14">

          <div class="timeline-line"></div>


          <!-- PENDIDIKAN -->

          <div class="relative pl-12 pb-12 reveal">

            <div class="absolute left-0 top-1 w-8 h-8 rounded-full bg-pink-500 text-white flex items-center justify-center">
              🎓
            </div>


            <div class="cute-card rounded-3xl p-7">

              <span class="text-sm text-pink-500 font-bold">
                PENDIDIKAN
              </span>

              <h3 class="text-2xl font-bold mt-2">
                SMKN 42 Jakarta
              </h3>

              <p class="text-gray-600 mt-3 leading-relaxed">

                Saya adalah seorang pelajar yang aktif, berjiwa juang,
                kreatif, dan tangguh. Saya terus berusaha mengembangkan
                kemampuan melalui proses belajar dan berbagai pengalaman.

              </p>

            </div>

          </div>


          <!-- PERSONAL VALUES -->

          <div class="relative pl-12 reveal">

            <div class="absolute left-0 top-1 w-8 h-8 rounded-full bg-pink-300 flex items-center justify-center">
              ✨
            </div>


            <div class="cute-card rounded-3xl p-7">

              <span class="text-sm text-pink-500 font-bold">
                PERSONAL VALUES
              </span>

              <h3 class="text-2xl font-bold mt-2">
                Aktif • Tangguh • Berjiwa Juang
              </h3>


              <div class="flex flex-wrap gap-3 mt-5">

                <span class="px-4 py-2 bg-pink-100 text-pink-600 rounded-full text-sm">
                  Kreatif 🎨
                </span>

                <span class="px-4 py-2 bg-pink-100 text-pink-600 rounded-full text-sm">
                  Aktif 🌸
                </span>

                <span class="px-4 py-2 bg-pink-100 text-pink-600 rounded-full text-sm">
                  Tangguh 💪
                </span>

                <span class="px-4 py-2 bg-pink-100 text-pink-600 rounded-full text-sm">
                  Mau Belajar 📚
                </span>

              </div>

            </div>

          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         MY MEMORIES
    ========================== -->

    <section id="foto"
             class="py-24 px-5 bg-white/50">

      <div class="max-w-7xl mx-auto">


        <div class="text-center reveal">

          <span class="text-pink-500 font-bold">
            📸 MY MEMORIES 📸
          </span>

          <h2 class="text-4xl font-bold mt-2">
            Galeri Foto
          </h2>

          <p class="text-gray-500 mt-3">
            Ada 9 memories kecil yang punya cerita 💗
          </p>

        </div>


        <div class="grid grid-cols-2 md:grid-cols-3 gap-4 mt-12">


          <!-- MEMORY 1 -->

          <div class="memory-card gallery-item rounded-3xl overflow-hidden photo-placeholder"
               onclick="openInfo(
                 'Little Pink Things',
                 'Parfum dan benda kecil yang punya tempat tersendiri dalam keseharian Jihan.',
                 'assets/images/memories-1.jpg'
               )">

            <img src="assets/images/memories-1.jpg"
                 alt="Little Pink Things"
                 class="gallery-img w-full h-64 object-cover">

          </div>


          <!-- MEMORY 2 -->

          <div class="memory-card gallery-item rounded-3xl overflow-hidden photo-placeholder"
               onclick="openInfo(
                 'A Soft Little Friend',
                 'Boneka kecil yang membawa kesan manis dan hangat dalam sebuah kenangan.',
                 'assets/images/memories-2.jpg'
               )">

            <img src="assets/images/memories-2.jpg"
                 alt="A Soft Little Friend"
                 class="gallery-img w-full h-64 object-cover">

          </div>


          <!-- MEMORY 3 -->

          <div class="memory-card gallery-item rounded-3xl overflow-hidden photo-placeholder"
               onclick="openInfo(
                 'A Sweet Keepsake',
                 'Bingkai dan kartu kecil yang terasa seperti potongan kenangan yang disimpan baik-baik.',
                 'assets/images/memories-3.jpg'
               )">

            <img src="assets/images/memories-3.jpg"
                 alt="A Sweet Keepsake"
                 class="gallery-img w-full h-64 object-cover">

          </div>


          <!-- MEMORY 4 -->

          <div class="memory-card gallery-item rounded-3xl overflow-hidden photo-placeholder"
               onclick="openInfo(
                 'Flowers & Pages',
                 'Bunga sederhana di antara halaman buku—kecil, tapi punya suasana yang cantik.',
                 'assets/images/memories-4.jpg'
               )">

            <img src="assets/images/memories-4.jpg"
                 alt="Flowers and Pages"
                 class="gallery-img w-full h-64 object-cover">

          </div>


          <!-- MEMORY 5 -->

          <div class="memory-card gallery-item rounded-3xl overflow-hidden photo-placeholder"
               onclick="openInfo(
                 'Quiet Reading Time',
                 'Buku-buku yang menemani waktu santai dan momen untuk menikmati cerita.',
                 'assets/images/memories-5.jpg'
               )">

            <img src="assets/images/memories-5.jpg"
                 alt="Quiet Reading Time"
                 class="gallery-img w-full h-64 object-cover">

          </div>


          <!-- MEMORY 6 -->

          <div class="memory-card gallery-item rounded-3xl overflow-hidden photo-placeholder"
               onclick="openInfo(
                 'Tiny Captured Moments',
                 'Kumpulan polaroid yang menyimpan potongan momen dalam bentuk foto kecil.',
                 'assets/images/memories-6.jpg'
               )">

            <img src="assets/images/memories-6.jpg"
                 alt="Tiny Captured Moments"
                 class="gallery-img w-full h-64 object-cover">

          </div>


          <!-- MEMORY 7 -->

          <div class="memory-card gallery-item rounded-3xl overflow-hidden photo-placeholder"
               onclick="openInfo(
                 'A Little Study Mood',
                 'Buku dan benda-benda kecil yang menemani suasana belajar dan aktivitas sehari-hari.',
                 'assets/images/memories-7.jpg'
               )">

            <img src="assets/images/memories-7.jpg"
                 alt="A Little Study Mood"
                 class="gallery-img w-full h-64 object-cover">

          </div>


          <!-- MEMORY 8 -->

          <div class="memory-card gallery-item rounded-3xl overflow-hidden photo-placeholder"
               onclick="openInfo(
                 'Getting Ready',
                 'Makeup dan little things yang menjadi bagian dari momen bersiap dan tampil percaya diri.',
                 'assets/images/memories-8.jpg'
               )">

            <img src="assets/images/memories-8.jpg"
                 alt="Getting Ready"
                 class="gallery-img w-full h-64 object-cover">

          </div>


          <!-- MEMORY 9 -->

          <div class="memory-card gallery-item rounded-3xl overflow-hidden photo-placeholder"
               onclick="openInfo(
                 'A Pink Ride',
                 'Bunga di dalam mobil pink—sebuah momen sederhana yang terlihat manis dan memorable.',
                 'assets/images/memories-9.jpg'
               )">

            <img src="assets/images/memories-9.jpg"
                 alt="A Pink Ride"
                 class="gallery-img w-full h-64 object-cover">

          </div>


        </div>

      </div>

    </section>


    <!-- =========================
         SOSIAL
    ========================== -->

    <section id="sosial"
             class="py-24 px-5">

      <div class="max-w-5xl mx-auto text-center">


        <div class="reveal">

          <span class="text-pink-500 font-bold">
            ♡ LET'S CONNECT ♡
          </span>

          <h2 class="text-4xl font-bold mt-2">
            Media Sosial
          </h2>

          <p class="text-gray-500 mt-3">
            Yuk terhubung denganku di media sosial! 🎀
          </p>

        </div>


        <div class="grid sm:grid-cols-2 gap-5 mt-12">


          <!-- INSTAGRAM -->

          <a href="https://www.instagram.com/xwlzz_yannsj/"
             target="_blank"
             rel="noopener noreferrer"
             class="social-btn cute-card rounded-3xl p-6 flex items-center gap-5 text-left">

            <div class="w-14 h-14 rounded-2xl bg-pink-100 text-pink-500 flex items-center justify-center text-2xl">

              <i class="fa-brands fa-instagram"></i>

            </div>


            <div>

              <h3 class="font-bold text-lg">
                Instagram
              </h3>

              <p class="text-gray-500">
                @xwlzz_yannsj
              </p>

            </div>


            <i class="fa-solid fa-arrow-up-right-from-square ml-auto text-pink-400"></i>

          </a>


          <!-- TIKTOK -->

          <a href="https://www.tiktok.com/@iluv_an0"
             target="_blank"
             rel="noopener noreferrer"
             class="social-btn cute-card rounded-3xl p-6 flex items-center gap-5 text-left">

            <div class="w-14 h-14 rounded-2xl bg-pink-100 text-pink-500 flex items-center justify-center text-2xl">

              <i class="fa-brands fa-tiktok"></i>

            </div>


            <div>

              <h3 class="font-bold text-lg">
                TikTok
              </h3>

              <p class="text-gray-500">
                @iluv_an0
              </p>

            </div>


            <i class="fa-solid fa-arrow-up-right-from-square ml-auto text-pink-400"></i>

          </a>


        </div>

      </div>

    </section>


    <!-- =========================
         KONTAK
    ========================== -->

    <section id="kontak"
             class="py-24 px-5">

      <div class="max-w-7xl mx-auto">


        <div class="text-center reveal">

          <span class="text-pink-500 font-bold">
            💌 CONTACT ME 💌
          </span>

          <h2 class="text-4xl font-bold mt-2">
            Hubungi Saya
          </h2>

        </div>


        <div class="grid lg:grid-cols-2 gap-8 mt-12">


          <!-- FORM -->

          <div class="cute-card rounded-[35px] p-7 reveal">

            <h3 class="text-2xl font-bold">
              Kirim Pesan 💗
            </h3>


            <form onsubmit="sendMessage(event)"
                  class="mt-7 space-y-5">


              <div>

                <label class="font-semibold text-sm">
                  Nama
                </label>

                <input id="name"
                       type="text"
                       required
                       placeholder="Nama kamu"
                       class="w-full mt-2 px-5 py-3 rounded-2xl border border-pink-100 outline-none focus:border-pink-400 bg-white">

              </div>


              <div>

                <label class="font-semibold text-sm">
                  Email
                </label>

                <input id="email"
                       type="email"
                       required
                       placeholder="email@example.com"
                       class="w-full mt-2 px-5 py-3 rounded-2xl border border-pink-100 outline-none focus:border-pink-400 bg-white">

              </div>


              <div>

                <label class="font-semibold text-sm">
                  Pesan
                </label>

                <textarea id="message"
                          rows="5"
                          required
                          placeholder="Tulis pesan..."
                          class="w-full mt-2 px-5 py-3 rounded-2xl border border-pink-100 outline-none focus:border-pink-400 bg-white"></textarea>

              </div>


              <button type="submit"
                      class="pink-btn w-full py-3 rounded-full font-bold">

                💌 Kirim Pesan

              </button>

            </form>

          </div>


          <!-- INFO KONTAK -->

          <div class="space-y-5 reveal">


            <!-- ALAMAT -->

            <div class="cute-card rounded-3xl p-6 flex gap-5">

              <div class="w-12 h-12 bg-pink-100 rounded-2xl flex items-center justify-center text-pink-500">

                <i class="fa-solid fa-location-dot"></i>

              </div>


              <div>

                <h3 class="font-bold">
                  Alamat
                </h3>

                <p class="text-gray-500 mt-1">
                  [ISI ALAMAT DI SINI]
                </p>

              </div>

            </div>


            <!-- EMAIL -->

            <div class="cute-card rounded-3xl p-6 flex gap-5">

              <div class="w-12 h-12 bg-pink-100 rounded-2xl flex items-center justify-center text-pink-500">

                <i class="fa-solid fa-envelope"></i>

              </div>


              <div>

                <h3 class="font-bold">
                  Email
                </h3>

                <a href="mailto:[EMAIL-KAMU]"
                   class="text-pink-500 hover:underline">

                  [EMAIL-KAMU]

                </a>

              </div>

            </div>


            <!-- WHATSAPP -->

            <div class="cute-card rounded-3xl p-6 flex gap-5">

              <div class="w-12 h-12 bg-pink-100 rounded-2xl flex items-center justify-center text-pink-500">

                <i class="fa-brands fa-whatsapp"></i>

              </div>


              <div>

                <h3 class="font-bold">
                  WhatsApp
                </h3>

                <a href="https://wa.me/[NOMOR-WA]"
                   target="_blank"
                   rel="noopener noreferrer"
                   class="text-pink-500 hover:underline">

                  Chat WhatsApp

                </a>

              </div>

            </div>


            <!-- GOOGLE MAPS -->

            <div class="cute-card rounded-3xl overflow-hidden h-72">

              <iframe
                title="Google Maps"
                src="https://www.google.com/maps?q=Jakarta%2C%20Indonesia&output=embed"
                width="100%"
                height="100%"
                style="border:0"
                loading="lazy"
                allowfullscreen>
              </iframe>

            </div>


          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         TESTIMONI
    ========================== -->

    <section id="testimoni"
             class="py-24 px-5 bg-white/50">

      <div class="max-w-4xl mx-auto text-center">


        <div class="reveal">

          <span class="text-pink-500 font-bold">
            💗 TESTIMONIAL 💗
          </span>

          <h2 class="text-4xl font-bold mt-2">
            Kata Mereka
          </h2>

        </div>


        <div class="cute-card rounded-[35px] p-8 mt-12 reveal">


          <div class="text-5xl mb-5">
            💗
          </div>


          <p id="testimonialText"
             class="text-lg text-gray-600 italic leading-relaxed">

            "Jihan adalah pribadi yang aktif,
            kreatif, dan memiliki semangat yang luar biasa."

          </p>


          <h3 id="testimonialName"
              class="font-bold text-xl mt-6">

            Testimoni 01

          </h3>


          <p id="testimonialRole"
             class="text-pink-500 text-sm mt-1">

            Teman

          </p>


          <div class="flex justify-center gap-3 mt-8">

            <button onclick="previousTestimonial()"
                    class="w-11 h-11 rounded-full bg-pink-100 text-pink-500">

              ←

            </button>


            <button onclick="nextTestimonial()"
                    class="w-11 h-11 rounded-full bg-pink-100 text-pink-500">

              →

            </button>

          </div>


        </div>

      </div>

    </section>

  </main>


  <!-- =========================
       FOOTER
  ========================== -->

  <footer class="py-10 px-5">

    <div class="max-w-7xl mx-auto text-center">


      <div class="cute-font text-2xl text-pink-500">

        Jihan Maharani Putri 🎀

      </div>


      <p class="text-gray-500 mt-3">

        Dibuat dengan ♡ dan sedikit glitter ✨

      </p>


      <div class="flex justify-center gap-4 mt-5 text-pink-400">

        <span>♡</span>
        <span>✦</span>
        <span>୨୧</span>
        <span>✧</span>
        <span>♡</span>

      </div>


      <p class="text-sm text-gray-400 mt-6">

        © 2026 Jihan Maharani Putri.
        All rights reserved.

      </p>

    </div>

  </footer>


  <!-- =========================
       MUSIC PLAYER
  ========================== -->

  <div class="music-player">

    <audio id="bgMusic" loop>

      <source
        src="assets/music/Semua-Aku-Dirayakan.mp3"
        type="audio/mpeg">

    </audio>


    <button id="musicBtn"
            onclick="toggleMusic()"
            class="w-14 h-14 rounded-full pink-btn flex items-center justify-center text-lg"
            title="Putar musik"
            aria-label="Putar atau jeda musik">

      <i id="musicIcon"
         class="fa-solid fa-music">
      </i>

    </button>

  </div>


  <!-- =========================
       POPUP HOBI + MEMORIES
  ========================== -->

  <div id="infoModal"
       class="hidden fixed inset-0 z-[9998] bg-black/60 backdrop-blur-sm items-center justify-center p-5"
       onclick="if(event.target===this)closeInfo()">


    <div class="cute-card max-w-md w-full rounded-[35px] p-5 relative">


      <button onclick="closeInfo()"
              class="absolute top-4 right-5 text-2xl text-pink-500"
              aria-label="Tutup">

        ×

      </button>


      <img id="infoImage"
           src=""
           alt=""
           class="w-full h-64 object-cover rounded-3xl">


      <div class="p-3 pt-5">

        <h3 id="infoTitle"
            class="text-2xl font-bold">
        </h3>


        <p id="infoDescription"
           class="text-gray-600 mt-3 leading-relaxed">
        </p>

      </div>

    </div>

  </div>


  <!-- =========================
       JAVASCRIPT
  ========================== -->

  <script>

    /* =========================
       MOBILE MENU
    ========================== */

    const menuBtn =
      document.getElementById("menuBtn");

    const mobileMenu =
      document.getElementById("mobileMenu");


    menuBtn.addEventListener("click", () => {

      mobileMenu.classList.toggle("show");

    });


    document
      .querySelectorAll("#mobileMenu a")
      .forEach(link => {

        link.addEventListener("click", () => {

          mobileMenu.classList.remove("show");

        });

      });


    /* =========================
       SCROLL REVEAL
    ========================== */

    const revealElements =
      document.querySelectorAll(".reveal");


    const observer =
      new IntersectionObserver(

        entries => {

          entries.forEach(entry => {

            if(entry.isIntersecting){

              entry.target.classList.add("active");

            }

          });

        },

        {
          threshold:0.12
        }

      );


    revealElements.forEach(element => {

      observer.observe(element);

    });


    /* =========================
       INFO MODAL
       HOBI + MEMORIES
    ========================== */

    const infoModal =
      document.getElementById("infoModal");

    const infoImage =
      document.getElementById("infoImage");

    const infoTitle =
      document.getElementById("infoTitle");

    const infoDescription =
      document.getElementById("infoDescription");


    function openInfo(
      title,
      description,
      image
    ){

      infoTitle.textContent =
        title;

      infoDescription.textContent =
        description;

      infoImage.src =
        image;

      infoModal.classList.remove("hidden");

      infoModal.classList.add("flex");

      document.body.style.overflow =
        "hidden";

    }


    function closeInfo(){

      infoModal.classList.add("hidden");

      infoModal.classList.remove("flex");

      infoImage.src =
        "";

      document.body.style.overflow =
        "";

    }


    /* =========================
       MUSIC
    ========================== */

    const music =
      document.getElementById("bgMusic");

    const musicIcon =
      document.getElementById("musicIcon");


    function toggleMusic(){

      if(music.paused){

        music.play()
          .then(() => {

            musicIcon.className =
              "fa-solid fa-pause";

          })

          .catch(() => {

            alert(
              "Pastikan file Semua-Aku-Dirayakan.mp3 sudah ada di folder assets/music/"
            );

          });

      }

      else{

        music.pause();

        musicIcon
