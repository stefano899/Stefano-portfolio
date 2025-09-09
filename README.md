<!doctype html>
<html lang="it">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Stefano's Portfolio</title>

  <!-- Bootstrap -->
  <link
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css"
    rel="stylesheet"
    integrity="sha384-9ndCyUa6mY5hYvY/2Qp2lG9GqQ8K/uxwD9GqvZf8BqC2J6m6k4l9Gd6Y4Z4SU1oF"
    crossorigin="anonymous"
  />

  <style>
    :root {
      /* Regola qui l'altezza globale delle card e dell'area testo */
      --card-height: 300px;      /* altezza totale del corpo card */
      --text-max-height: 170px;  /* altezza dell'area scrollabile */
    }

    body { background-color: #f8f9fa; }

    .profile-img {
      width: 150px;
      height: 150px;
      object-fit: cover;
      border-radius: 50%;
      border: 4px solid #0d6efd;
    }

    .portfolio-card { transition: transform 0.3s ease; }
    .portfolio-card:hover { transform: translateY(-5px); }

    /* Card uniformi + layout per allineare il bottone in basso */
    .portfolio-card .card-body {
      height: var(--card-height);
      display: flex;
      flex-direction: column;
    }

    /* Area descrizione scrollabile */
    .card-text-scroll {
      flex: 1 1 auto;
      overflow: auto;
      max-height: var(--text-max-height);
    }

    /* Spazio tra testo e bottone, bottone parte da sinistra */
    .card-body .btn {
      margin-top: 0.75rem;
      align-self: flex-start;
    }

    /* Piccolo tuning responsive: su schermi piccoli alzo l'area testo (puoi regolare) */
    @media (max-width: 575.98px) {
      :root {
        --card-height: 320px;
        --text-max-height: 200px;
      }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header class="bg-white shadow-sm py-4 mb-5">
    <div class="container text-center">
      <img
        src="profilo.jpg"
        alt="Foto profilo di Stefano Rosini"
        class="profile-img mb-3"
      />
      <h1 class="fw-bold">Stefano Rosini</h1>
      <p class="lead mb-1">Computer Scientist | Master's Student in Computer Science</p>
      <p class="mb-0">I have a passion for learning new things and I can adapt easily to new environments.</p>
    </div>
  </header>

  <!-- Portfolio -->
  <section class="container mb-5">
    <h2 class="text-center mb-4">Portfolio Projects</h2>
    <div class="row g-4">
      <!-- Card 1 -->
      <div class="col-md-6 col-lg-4">
        <div class="card portfolio-card shadow-sm h-100">
          <div class="card-body">
            <h5 class="card-title">Periodontitis Detection</h5>
            <div class="card-text-scroll">
              A study from my bachelor's thesis in which I used smartphone images and MATLAB image processing methods to automatically detect and segment teeth for periodontitis evaluation. The whole project was built in MATLAB.
            </div>
            <a
              href="https://ieeexplore.ieee.org/document/10178731"
              class="btn btn-outline-primary"
              target="_blank"
              rel="noopener noreferrer"
            >Read Paper</a>
          </div>
        </div>
      </div>
      <!-- Card 2 -->
      <div class="col-md-6 col-lg-4">
        <div class="card portfolio-card shadow-sm h-100">
          <div class="card-body">
            <h5 class="card-title">Agent Implementation</h5>
            <div class="card-text-scroll">
              Project from my master's degree: I used DALI
              (<a href="https://stefano899.github.io/Stefano-portfolio/" target="_blank" rel="noopener noreferrer">link to the DALI paper</a>)
              to create intelligent agents that cooperate to run an auction.
            </div>
            <a
              href="https://github.com/stefano899/AgentArchitecture"
              class="btn btn-outline-primary"
              target="_blank"
              rel="noopener noreferrer"
            >Go to the project</a>
          </div>
        </div>
      </div>
      <!-- Card 3 -->
      <div class="col-md-6 col-lg-4">
        <div class="card portfolio-card shadow-sm h-100">
          <div class="card-body">
            <h5 class="card-title">Python CNN Implementation</h5>
            <div class="card-text-scroll">
              Project from my master's degree: I created two CNN architectures with different initialization schemes to compare their performance.
            </div>
            <a
              href="https://github.com/stefano899/DNN_2025"
              class="btn btn-outline-primary"
              target="_blank"
              rel="noopener noreferrer"
            >Go to the project</a>
          </div>
        </div>
      </div>
      <!-- Card 4 -->
      <div class="col-md-6 col-lg-4">
        <div class="card portfolio-card shadow-sm h-100">
          <div class="card-body">
            <h5 class="card-title">Java Chess Implementation</h5>
            <div class="card-text-scroll">
              A simple terminal-based chess game developed during my bachelor's degree, using Java and the Java Collections Framework.
            </div>
            <a
              href="https://github.com/LPODISIM2023/scacchi-informatici-a-chiamata"
              class="btn btn-outline-primary"
              target="_blank"
              rel="noopener noreferrer"
            >Go to the project</a>
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
              <ul class="mb-2">
                <li><strong>PhishingFinale</strong>: Built a binary decision tree classifier to distinguish between phishing and non-phishing websites, with statistical analysis to assess whether dataset manipulation was needed.</li>
                <li><strong>Challenge Avezzano &amp; Pescara (2 projects)</strong>: Predicted contract sales for cities in the Abruzzo region and designed a decision optimization algorithm to estimate the optimal backbone network rooted in Avezzano and Pescara. The two codes share the same data analysis.</li>
              </ul>
              Technologies used: Python (scikit-learn, pandas, gurobipy).
            </div>
            <a
              href="https://github.com/stefano899/Data-Science-Project"
              class="btn btn-outline-primary"
              target="_blank"
              rel="noopener noreferrer"
            >Go to the project</a>
          </div>
        </div>
      </div>
      <!-- Card 6 -->
      <div class="col-md-6 col-lg-4">
        <div class="card portfolio-card shadow-sm h-100">
          <div class="card-body">
            <h5 class="card-title">Dataset Analysis Projects</h5>
            <div class="card-text-scroll">
              Some projects where I used pandas and NannyML for analyzing datasets.
            </div>
            <a
              href="https://github.com/stefano899/Dataset-Analisys"
              class="btn btn-outline-primary"
              target="_blank"
              rel="noopener noreferrer"
            >Go to the project</a>
          </div>
        </div>
      </div>
      <!-- Card 7 -->
      <div class="col-md-6 col-lg-4">
        <div class="card portfolio-card shadow-sm h-100">
          <div class="card-body">
            <h5 class="card-title">Machine Learning Projects</h5>
            <div class="card-text-scroll">
              Machine learning projects done during the master's in Computer Science. This repo contains three projects:
              <ul class="mb-2">
                <li><strong>Missing Values Predictor</strong>: a model to predict missing values in a dataset.</li>
                <li><strong>Sequence Predictors</strong>: algorithms to predict sequences of symbolic or numeric values given an observed sequence.</li>
                <li><strong>Objects Recognition</strong>: ML algorithms for classifying objects from a given dataset.</li>
              </ul>
              More information is available in the documentation files within each project folder.
            </div>
            <a
              href="https://github.com/stefano899/Dataset-Analisys"
              class="btn btn-outline-primary"
              target="_blank"
              rel="noopener noreferrer"
            >Go to the project</a>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- Footer -->
  <footer class="text-center py-4">
    <a
      href="https://scholar.google.com/citations?user=zHYgI1QAAAAJ&hl=it&oi=ao"
      class="btn btn-primary mx-2"
      target="_blank"
      rel="noopener noreferrer"
    >Scholar Page</a>
  </footer>

  <!-- Bootstrap JS (opzionale, per componenti interattivi) -->
  <script
    src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"
    integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8Y7B1zYkGmQm5t1QK04YgG6F"
    crossorigin="anonymous"
  ></script>
</body>
</html>
