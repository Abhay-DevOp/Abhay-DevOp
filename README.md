<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>DevOps Engineer - GitHub Profile Dashboard</title>

<style>
    body {
        margin: 0;
        font-family: "Inter", sans-serif;
        background: linear-gradient(135deg, #0f0f0f, #1b1b1b);
        color: #fff;
    }

    .header {
        text-align: center;
        padding: 50px 20px;
    }

    .header h1 {
        font-size: 3rem;
        margin-bottom: 10px;
    }

    .header p {
        font-size: 1.2rem;
        opacity: 0.8;
    }

    /* Card Layout */
    .container {
        width: 90%;
        max-width: 1100px;
        margin: auto;
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 25px;
        padding-bottom: 50px;
    }

    .card {
        background: rgba(255, 255, 255, 0.08);
        backdrop-filter: blur(10px);
        padding: 25px;
        border-radius: 15px;
        box-shadow: 0 8px 20px rgba(0,0,0,0.3);
        transition: 0.3s;
    }

    .card:hover {
        transform: translateY(-5px);
        background: rgba(255, 255, 255, 0.12);
    }

    .card h2 {
        margin-bottom: 15px;
    }

    .skills span {
        display: inline-block;
        padding: 8px 12px;
        background: #111;
        margin: 4px;
        border-radius: 8px;
        font-size: 0.9rem;
        border: 1px solid #333;
    }

    /* Timeline */
    .timeline {
        border-left: 3px solid #00d4ff;
        margin-left: 15px;
        padding-left: 20px;
    }

    .timeline-item {
        margin-bottom: 20px;
    }

    .timeline-item h3 {
        margin: 0;
        color: #00d4ff;
    }

    /* Footer */
    .footer {
        text-align: center;
        padding: 30px;
        opacity: 0.6;
    }

    /* Social icons */
    .social a {
        margin: 0 8px;
        display: inline-block;
        filter: brightness(0) invert(1);
    }
</style>

</head>
<body>

<!-- HEADER -->
<div class="header">
    <h1>👨‍💻 Your Name</h1>
    <p>DevOps Engineer | Cloud | Automation | CI/CD | SRE</p>

    <div class="social">
        <a href="#"><img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/github.svg" width="28"></a>
        <a href="#"><img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/linkedin.svg" width="28"></a>
        <a href="#"><img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/docker.svg" width="28"></a>
        <a href="#"><img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/kubernetes.svg" width="28"></a>
    </div>
</div>

<!-- DASHBOARD GRID -->
<div class="container">

    <!-- GitHub Stats -->
    <div class="card">
        <h2>📊 GitHub Stats</h2>
        <img src="https://github-readme-stats.vercel.app/api?username=USERNAME&show_icons=true&theme=tokyonight" width="100%">
        <br><br>
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=USERNAME&theme=tokyonight" width="100%">
    </div>

    <!-- Tech Stack -->
    <div class="card">
        <h2>⚙️ DevOps Tech Stack</h2>
        <div class="skills">
            <span>AWS</span><span>Azure</span><span>GCP</span>
            <span>Docker</span><span>Kubernetes</span><span>Helm</span>
            <span>Ansible</span><span>Terraform</span><span>Jenkins</span>
            <span>GitHub Actions</span><span>Linux</span>
        </div>
    </div>

    <!-- Projects -->
    <div class="card">
        <h2>🚀 Featured Projects</h2>
        <ul>
            <li><b>CI/CD Pipeline Automation:</b> End-to-end GitHub Actions pipeline.</li>
            <li><b>K8s Microservices Deployment:</b> Helm + ArgoCD.</li>
            <li><b>Infrastructure-as-Code:</b> Terraform AWS VPC + EKS setup.</li>
        </ul>
    </div>

    <!-- Experience Timeline -->
    <div class="card">
        <h2>📅 Experience</h2>
        <div class="timeline">
            <div class="timeline-item">
                <h3>DevOps Engineer</h3>
                <p>2022 - Present | Company Name</p>
            </div>
            <div class="timeline-item">
                <h3>Cloud / SRE Intern</h3>
                <p>2021 - 2022 | Company</p>
            </div>
        </div>
    </div>

    <!-- Contact Card -->
    <div class="card">
        <h2>📨 Contact</h2>
        <p>Email: <b>you@example.com</b></p>
        <p>Portfolio: yourwebsite.com</p>
        <p>Location: 🌍 Earth</p>
    </div>

</div>

<div class="footer">
    © 2025 Your Name — DevOps Engineer Dashboard
</div>

</body>
</html>
