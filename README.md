<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stefano's Portfolio</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background-color: #f8f9fa;
        }
        .profile-img {
            width: 150px;
            height: 150px;
            object-fit: cover;
            border-radius: 50%;
            border: 4px solid #0d6efd;
        }
        .portfolio-card {
            transition: transform 0.3s ease;
        }
        .portfolio-card:hover {
            transform: translateY(-5px);
        }
    </style>
</head>
<body>

<!-- Header Section -->
<header class="bg-white shadow-sm py-4 mb-5">
    <div class="container text-center">
        <img src="profilo.jpg" alt="Profile Picture" class="profile-img mb-3">
        <h1 class="fw-bold">Stefano Rosini</h1>
        <p class="lead">Computer Scientist | Master's Student in Computer Science</p>
        <p>I have a passion for learning new things and i can adapt easily to new environments.</p>
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
                        A study made during the bachelor's thesys in which i used Smartphone images and MATLAB image processing methods to automatically detect and segment teeth for periodontitis evaluation.
                    </p>
                    <a href="https://ieeexplore.ieee.org/document/10178731" class="btn btn-outline-primary" target="_blank">Read Paper</a>
                </div>
            </div>
        </div>
        <!-- Add more cards here -->
        <div class="col-md-6 col-lg-4">
            <div class="card portfolio-card shadow-sm h-100">
                <div class="card-body">
                    <h5 class="card-title">Agent Implementation</h5>
                    <p class="card-text">In this project made during the master's degree, i made a project in DALI (<a href="https://stefano899.github.io/Stefano-portfolio/">Link to the DALI's paper</a>) in which i created some intelligents agents that cooperate with eachothers into doing an auction.</p>
                    <a href="https://github.com/stefano899/AgentArchitecture" class="btn btn-outline-primary" target="_blank">Go to the project</a>
                </div>
            </div>
        </div>
        <div class="col-md-6 col-lg-4">
            <div class="card portfolio-card shadow-sm h-100">
                <div class="card-body">
                    <h5 class="card-title">Python CNN Implementation</h5>
                    <p class="card-text">In this project made during the master's degree, i created 2 CNN architectures with different initialization schemas for the evaluation of the performances between them.</p>
                    <a href="https://github.com/stefano899/DNN_2025" class="btn btn-outline-primary" target="_blank">Go to the project</a>
                </div>
            </div>
        </div>
        <div class="col-md-6 col-lg-4">
            <div class="card portfolio-card shadow-sm h-100">
                <div class="card-body">
                    <h5 class="card-title">Java Chess Implementation</h5>
                    <p class="card-text">In this project made during my bachelor's degree, i made a project in Java in which i created a simple chess game that runs on terminal.</p>
                    <a href="https://github.com/LPODISIM2023/scacchi-informatici-a-chiamata" class="btn btn-outline-primary" target="_blank">Go to the project</a>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Footer Links -->
<footer class="text-center py-4">
    <a href="https://stefano899.github.io/Stefano-portfolio/" class="btn btn-primary mx-2" target="_blank">Visit My Full Site</a>
    <a href="https://scholar.google.com/citations?user=zHYgI1QAAAAJ&hl=it&oi=ao" class="btn btn-outline-secondary mx-2" target="_blank"> Scholar Page</a>
</footer>

</body>
</html>
