<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Stefano's Portfolio</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" />
  <style>
    body { background-color: #f8f9fa; }
    .profile-img {
      width: 150px; height: 150px; object-fit: cover;
      border-radius: 50%; border: 4px solid #0d6efd;
    }
    .portfolio-card { transition: transform 0.3s ease; }
    .portfolio-card:hover { transform: translateY(-5px); }
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
    <!-- Project Card 1 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Periodontitis Detection (MATLAB)</h5>
          <p class="card-text">
            Bachelor's thesis: smartphone images + MATLAB image processing to detect and segment teeth for periodontitis evaluation.
          </p>
          <a href="https://ieeexplore.ieee.org/document/10178731" class="btn btn-outline-primary" target="_blank" rel="noopener">Read Paper</a>
        </div>
      </div>
    </div>

    <!-- Project Card 2 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Agent Implementation</h5>
          <p class="card-text">
            DALI project: a set of intelligent agents cooperating to run an auction.
            (<a href="https://stefano899.github.io/Stefano-portfolio/" target="_blank" rel="noopener">About DALI</a>)
          </p>
          <a href="https://github.com/stefano899/AgentArchitecture" class="btn btn-outline-primary" target="_blank" rel="noopener">Go to the project</a>
        </div>
      </div>
    </div>

    <!-- Project Card 3 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Python CNN Implementation</h5>
          <p class="card-text">Two CNN architectures with different initializations to compare performance.</p>
          <a href="https://github.com/stefano899/DNN_2025" class="btn btn-outline-primary" target="_blank" rel="noopener">Go to the project</a>
        </div>
      </div>
    </div>

    <!-- Project Card 4 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Java Chess Implementation</h5>
          <p class="card-text">Simple terminal chess game (Bachelor's project) written in Java.</p>
          <a href="https://github.com/LPODISIM2023/scacchi-informatici-a-chiamata" class="btn btn-outline-primary" target="_blank" rel="noopener">Go to the project</a>
        </div>
      </div>
    </div>

    <!-- Project Card 5 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Data-Science-Project</h5>
          <p class="card-text">
            Phishing classifier (Decision Tree + stats) and sales forecasting/optimization (Avezzano/Pescara).
            Python: scikit-learn, pandas, gurobipy.
          </p>
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
