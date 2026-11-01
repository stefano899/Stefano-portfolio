<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Stefano's Portfolio</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" />
  <style>
    :root{
      /* regola qui l'altezza del corpo di tutte le card */
      --card-height: 320px;
    }
    body { background-color: #f8f9fa; }
    .profile-img {
      width: 150px; height: 150px; object-fit: cover;
      border-radius: 50%; border: 4px solid #0d6efd;
    }
    .portfolio-card { transition: transform 0.3s ease; }
    .portfolio-card:hover { transform: translateY(-5px); }
    /* Card tutte alte uguali: titolo in alto, bottone sempre in fondo */
    .portfolio-card .card-body{
      height: var(--card-height);
      display: flex;
      flex-direction: column;
    }
    /* L'area testo occupa lo spazio rimasto e scorre se il testo è lungo */
    .card-text-scroll{
      flex: 1 1 auto;
      min-height: 0;
      overflow-y: auto;
    }
    .card-text-scroll ul{
      padding-left: 1.2rem;
      margin-bottom: 0.5rem;
    }
    /* Spazio tra testo e bottone, bottone parte da sinistra */
    .card-body .btn{
      margin-top: 0.75rem;
      align-self: flex-start;
    }
    /* Su schermi piccoli c'è una card per riga: altezza in base al contenuto */
    @media (max-width: 767.98px){
      .portfolio-card .card-body{ height: auto; }
      .card-text-scroll{ max-height: 220px; }
    }
  </style>
</head>
<body>
<!-- Header Section -->
<header class="bg-white shadow-sm py-4 mb-5">
  <div class="container text-center">
    <img src="profilo.jpg" alt="Profile photo of Stefano Rosini" class="profile-img mb-3" />
    <h1 class="fw-bold">Stefano Rosini</h1>
    <p class="lead">Research Fellow in AI for Medical Imaging | MSc in Computer Science</p>
    <p>I have a passion for learning new things and I adapt easily to new environments.</p>
  </div>
</header>
<!-- Portfolio Section -->
<section class="container mb-5">
  <h2 class="text-center mb-4">Portfolio Projects</h2>
  <div class="row g-4 justify-content-center">
    <!-- Card 1 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Periodontitis Detection</h5>
          <div class="card-text-scroll">
            A study carried out for my bachelor's thesis, in which I used smartphone images and image processing methods to automatically detect and segment teeth for periodontitis evaluation. The whole project was developed in MATLAB.
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
            A project developed during my master's degree in DALI (<a href="https://github.com/AAAI-DISIM-UnivAQ/DALI/blob/master/docs/DALI_Language_description.pdf" target="_blank" rel="noopener">DALI paper</a>), in which I created intelligent agents that cooperate with each other to run an auction.
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
            A project developed during my master's degree, in which I built two CNN architectures with different initialization schemes and compared their performance.
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
            A simple terminal-based chess game developed during my bachelor's degree, using Java and the Java Collections Framework.
          </div>
          <a href="https://github.com/LPODISIM2023/scacchi-informatici-a-chiamata" class="btn btn-outline-primary" target="_blank" rel="noopener">Go to the project</a>
        </div>
      </div>
    </div>
    <!-- Card 5 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Data Science Project</h5>
          <div class="card-text-scroll">
            For the Data Analytics and Data-Driven Decision exam, I developed three projects:
            <ul>
              <li><b>PhishingFinale</b>: a binary decision tree classifier that distinguishes phishing from non-phishing websites, supported by a statistical analysis to decide whether the dataset needed to be manipulated.</li>
              <li><b>Challenge Avezzano &amp; Pescara (2 projects)</b>: predicted contract sales for cities in the Abruzzo region and designed a decision optimization algorithm to estimate the optimal backbone network rooted in Avezzano and Pescara. Both projects share the same data analysis.</li>
            </ul>
            Technologies: Python (Scikit-learn, Pandas, GurobiPy).
          </div>
          <a href="https://github.com/stefano899/Data-Science-Project" class="btn btn-outline-primary" target="_blank" rel="noopener">Go to the project</a>
        </div>
      </div>
    </div>
    <!-- Card 6 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Dataset Analysis Projects</h5>
          <div class="card-text-scroll">
            Projects in which I used Pandas and NannyML to analyze datasets.
          </div>
          <a href="https://github.com/stefano899/Dataset-Analisys" class="btn btn-outline-primary" target="_blank" rel="noopener">Go to the project</a>
        </div>
      </div>
    </div>
    <!-- Card 7 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">Machine Learning Projects</h5>
          <div class="card-text-scroll">
            Machine learning projects developed during my master's degree in computer science. The repository contains three projects:
            <ul>
              <li><b>Missing values predictor</b>: a machine learning model that predicts missing values in a dataset.</li>
              <li><b>Sequence predictors</b>: algorithms that predict sequences of symbolic or numeric values, given a known sequence.</li>
              <li><b>Object recognition</b>: machine learning algorithms that classify objects from a given dataset.</li>
            </ul>
            More details are available in the documentation inside each project folder.
          </div>
          <a href="https://github.com/stefano899/Machine-Learning" class="btn btn-outline-primary" target="_blank" rel="noopener">Go to the project</a>
        </div>
      </div>
    </div>
    <!-- Card 8 -->
    <div class="col-md-6 col-lg-4">
      <div class="card portfolio-card shadow-sm h-100">
        <div class="card-body">
          <h5 class="card-title">RAG Cooking Assistant</h5>
          <div class="card-text-scroll">
            A Retrieval-Augmented Generation (RAG) assistant that answers cooking questions using Italian recipe books:
            <ul>
              <li>the PDF recipe books are converted to Markdown and split into one chunk per recipe;</li>
              <li>the recipes are embedded and stored in a ChromaDB vector database;</li>
              <li>for each question, the closest recipes are retrieved and passed to an LLM (Gemini), which answers citing the recipes it used as sources.</li>
            </ul>
            The project runs in a Docker dev container.
            Technologies: Python (ChromaDB, PyMuPDF4LLM, OpenAI SDK), Docker.
          </div>
          <a href="https://github.com/stefano899/rag-cucina" class="btn btn-outline-primary" target="_blank" rel="noopener">Go to the project</a>
        </div>
      </div>
    </div>
  </div>
</section>
<!-- Footer Links -->
<footer class="text-center py-4">
  <a href="https://scholar.google.com/citations?user=zHYgI1QAAAAJ&amp;hl=it&amp;oi=ao" class="btn btn-primary mx-2" target="_blank" rel="noopener">Scholar Page</a>
</footer>
</body>
</html>
