<html lang="it">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Stefano's Portfolio</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" />
  <style>
    :root{
      /* regola qui l'altezza globale delle card e dell'area testo */
      --card-height: 300px;      /* altezza totale card (solo il corpo) */
      --text-max-height: 170px;  /* altezza dell'area scrollabile */
    }
    body { background-color: #f8f9fa; }
    .profile-img {
      width: 150px; height: 150px; object-fit: cover;
      border-radius: 50%; border: 4px solid #0d6efd;
    }
    .portfolio-card { transition: transform 0.3s ease; }
    .portfolio-card:hover { transform: translateY(-5px); }
    /* Card uniformi + layout per allineare il bottone in basso */
    .portfolio-card .card-body{
      height: var(--card-height);
      display: flex;
      flex-direction: column;
    }
    /* Area descrizione scrollabile */
    .card-text-scroll{
      flex: 1 1 auto;
      overflow: auto;
      max-height: var(--text-max-height);
    }
    /* Spazio tra testo e bottone, bottone parte da sinistra */
    .card-body .btn{
      margin-top: 0.75rem;
      align-self: flex-start;
    }
    /* Piccolo tuning responsive: su schermi piccoli alzo l'area testo */
    @media (max-width: 575.98px){
      :root{
        --card-height: 300px;
        --text-max-height: 170px;
      }
    }
  </style>
</head>
<body>
<!-- Header Section -->
<header class="bg-white shadow-sm py-4 mb-5">
  <div class="container text-center">
    <img src="profilo.jpg" alt="Foto profilo di Stefano Rosini" class="profile-img mb-3" />
    <h1 class="fw-bold">Stefano Rosini</h1>
    <p class="lead">Computer Scientist | Master's Student in Computer Science</p>
    <p>I have a passion for learning new things and I can adapt easily to new environments.</p>
  </div>
</header>

<!-- Portfolio Section -->
<section class="container mb-5">
  <h2 class="text-center mb-4">Portfolio Projects</h2>

  <div class="row g-4">
    <!-- Card 1 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Periodontitis Detection </h5>
          <div class="card-text-scroll">
            A study made during the bachelor's thesys in which i used Smartphone images and MATLAB image processing methods to automatically detect and segment teeth for periodontitis evaluation. The whole project was made in MATLAB
          </div>
          <a href="https://ieeexplore.ieee.org/document/10178731" class="btn btn-outline-primary" target="_blank" rel="noopener">Read Paper</a>
        </div>
      </div>
    </div>
    <!-- Card 2 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Agent Implementation</h5>
          <div class="card-text-scroll">
            In this project made during the master's degree, i made a project in DALI (<a href="https://stefano899.github.io/Stefano-portfolio/">Link to the DALI's paper</a>) in which i created some intelligents agents that cooperate with eachothers into doing an auction.
          </div>
          <a href="https://github.com/stefano899/AgentArchitecture" class="btn btn-outline-primary" target="_blank" rel="noopener">Go to the project</a>
        </div>
      </div>
    </div>
    <!-- Card 3 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Python CNN Implementation</h5>
          <div class="card-text-scroll">
            In this project made during the master's degree, i created 2 CNN architectures with different initialization schemas for the evaluation of the performances between them.
          </div>
          <a href="https://github.com/stefano899/DNN_2025" class="btn btn-outline-primary" target="_blank" rel="noopener">Go to the project</a>
        </div>
      </div>
    </div>
    <!-- Card 4 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Java Chess Implementation</h5>
          <div class="card-text-scroll">
             A simple terminal-based chess game developed during my Bachelor's degree, using Java and the Java Collections Framework.
          </div>
          <a href="https://github.com/LPODISIM2023/scacchi-informatici-a-chiamata" class="btn btn-outline-primary" target="_blank" rel="noopener">Go to the project</a>
        </div>
      </div>
    </div>
    <!-- Card 5 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Data-Science-Project</h5>
          <div class="card-text-scroll">
            For the Data Analytics and Data-Driven Decision exam, I developed three projects:
<ul>
PhishingFinale: Built a binary decision tree classifier to distinguish between phishing and non-phishing websites, supported by statistical analysis for deciding if the dataset should have been manipulated or not.

Challenge Avezzano & Pescara(2 projects): Predicted contract sales for cities in the Abruzzo region and designed a decision optimization algorithm to estimate the optimal backbone network based on the dataset with root in Avezzano and Pescara. The two codes have the same data analysis.
</ul>
Technologies used: Python Libraries: Scikit-learn, Pandas, GurobiPy
          </div>
          <a href="https://github.com/stefano899/Data-Science-Project" class="btn btn-outline-primary" target="_blank" rel="noopener">Go to the project</a>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Footer Links -->
<footer class="text-center py-4">
  <a href="https://scholar.google.com/citations?user=zHYgI1QAAAAJ&hl=it&oi=ao" class="btn btn-primary mx-2" target="_blank" rel="noopener">Scholar Page</a>
</footer>

</body>
</html>
