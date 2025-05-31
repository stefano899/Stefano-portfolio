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
        <p>I have a passion for learning new things and can adapt easily to new environments.</p>
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
                        A study using smartphone images and MATLAB to automatically detect and segment teeth for periodontitis evaluation.
                    </p>
                    <a href="https://ieeexplore.ieee.org/document/10178731" class="btn btn-outline-primary" target="_blank">Read Paper</a>
                </div>
            </div>
        </div>

        <!-- Add more cards here -->
        <!-- Example:
        <div class="col-md-6 col-lg-4">
            <div class="card portfolio-card shadow-sm h-100">
                <div class="card-body">
                    <h5 class="card-title">Project Title</h5>
                    <p class="card-text">Short description of the project.</p>
                    <a href="#" class="btn btn-outline-primary" target="_blank">View More</a>
                </div>
            </div>
        </div>
        -->

    </div>
</section>

<!-- Footer Links -->
<footer class="text-center py-4">
    <a href="https://stefano899.github.io/Stefano-portfolio/" class="btn btn-primary mx-2" target="_blank">Visit My Full Site</a>
    <a href="https://ieeexplore.ieee.org/document/10178731" class="btn btn-outline-secondary mx-2" target="_blank">Published Paper</a>
</footer>

</body>
</html>
