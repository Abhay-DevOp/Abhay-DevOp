<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Abhay Agarwal | DevOps Engineer Dashboard</title>

<!-- Chart.js for animated charts -->
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<style>
    body {
        margin: 0;
        font-family: "Inter", sans-serif;
        background: #f5f7fa;
        color: #222;
    }

    .header {
        text-align: center;
        padding: 50px 20px;
        background: #e9f1ff;
        border-bottom: 2px solid #d0dff7;
    }

    .header h1 {
        font-size: 3rem;
        font-weight: 800;
        color: #0b4fff;
    }

    .header p {
        font-size: 1.2rem;
        opacity: 0.7;
        margin-top: -10px;
    }

    .container {
        width: 90%;
        max-width: 1150px;
        margin: auto;
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(330px, 1fr));
        gap: 25px;
        padding: 40px 0;
    }

    .card {
        background: #ffffff;
        padding: 25px;
        border-radius: 15px;
        box-shadow: 0 4px 15px rgba(0,0,0,0.08);
        border: 1px solid #e4e9f0;
        transition: 0.25s;
    }

    .card:hover {
        transform: translateY(-5px);
        box-shadow: 0 8px 20px rgba(0,0,0,0.12);
    }

    .card h2 {
        color: #0b4fff;
        margin-bottom: 15px;
        font-weight: 700;
    }

    .skills span {
        display: inline-block;
        padding: 8px 12px;
        background: #eaf0ff;
        color: #0037cc;
        margin: 4px;
        border-radius: 8px;
        font-size: 0.85rem;
        border: 1px solid #d1dbff;
        font-weight: 600;
    }

    .timeline {
        border-left: 3px solid #0b4fff;
        padding-left: 20px;
    }

    .timeline-item {
        margin-bottom: 20px;
    }

    .timeline-item h3 {
        margin: 0;
        color: #0b4fff;
    }

    .docker-k8s-badge {
        display: flex;
        gap: 20px;
        margin: 20px 0;
        justify-content: center;
    }

    .docker-k8s-badge img {
        width: 70px;
        opacity: 0.9;
    }

    .footer {
        text-align: center;
        padding: 30px;
        opacity: 0.6;
        border-top: 1px solid #ddd;
        margin-top: 40px;
    }
</style>
</head>
<body>

<!-- HEADER -->
<div class="header">
    <h1>Abhay Agarwal</h1>
    <p>DevOps Engineer • Cloud • CI/CD • SRE • Automation</p>

    <div class="docker-k8s-badge">
        <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/docker.svg">
        <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/kubernetes.svg">
    </div>
</div>

<!-- GRID -->
<div class="container">

    <!-- GitHub Stats -->
    <div class="card">
        <h2>📊 GitHub Stats</h2>
        <img src="https://github-readme-stats.vercel.app/api?username=YOUR_GITHUB_USERNAME&show_icons=true&theme=default" width="100%">
        <br><br>
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=YOUR_GITHUB_USERNAME&theme=default" width="100%">
    </div>

    <!-- Animated Skills Chart -->
    <div class="card">
        <h2>📈 DevOps Skills Chart (Animated)</h2>
        <canvas id="skillsChart"></canvas>
    </div>

    <!-- Tech Stack -->
    <div class="card">
        <h2>⚙️ DevOps Tech Stack</h2>
        <div class="skills">
            <span>AWS</span><span>Azure</span><span>GCP</span>
            <span>Docker</span><span>Kubernetes</span><span>Helm</span>
            <span>Terraform</span><span>Ansible</span><span>Jenkins</span>
            <span>GitHub Actions</span><span>Linux</span><span>Prometheus</span>
        </div>
    </div>

    <!-- Certifications -->
    <div class="card">
        <h2>🎓 Certifications</h2>
        <ul>
            <li>AWS Certified Solutions Architect – Associate</li>
            <li>CKA – Certified Kubernetes Administrator</li>
            <li>Terraform Associate (HashiCorp)</li>
            <li>Microsoft Azure Fundamentals AZ-900</li>
            <li>Docker Kubernetes Essentials</li>
        </ul>
    </div>

    <!-- Projects -->
    <div class="card">
        <h2>🚀 Featured Projects</h2>
        <ul>
            <li><b>Automated CI/CD Pipeline:</b> GitHub Actions + Terraform + AWS ECS</li>
            <li><b>Kubernetes Microservices Deployment:</b> Helm + ArgoCD + Ingress</li>
            <li><b>Infra-as-Code:</b> Full AWS VPC + EKS deployment via Terraform</li>
            <li><b>Monitoring Stack:</b> Prometheus + Grafana + Loki</li>
        </ul>
    </div>

    <!-- Experience -->
    <div class="card">
        <h2>📅 Professional Experience</h2>
        <div class="timeline">
            <div class="timeline-item">
                <h3>DevOps Engineer</h3>
                <p>2022 – Present | Company Name</p>
            </div>
            <div class="timeline-item">
                <h3>Cloud / SRE Intern</h3>
                <p>2021 – 2022 | Company Name</p>
            </div>
        </div>
    </div>

    <!-- Contact -->
    <div class="card">
        <h2>📨 Contact</h2>
        <p>Email: <b>abhay@example.com</b></p>
        <p>Portfolio: abhayagarwal.dev (optional)</p>
        <p>Location: India</p>
    </div>

</div>

<!-- FOOTER -->
<div class="footer">
    © 2025 Abhay Agarwal — DevOps Engineer Dashboard
</div>

<!-- CHART.JS SCRIPT -->
<script>
const ctx = document.getElementById('skillsChart');
new Chart(ctx, {
    type: 'radar',
    data: {
        labels: ['Docker', 'Kubernetes', 'Terraform', 'AWS', 'CI/CD', 'Linux', 'SRE'],
        datasets: [{
            label: 'Skill Level',
            data: [95, 90, 85, 92, 88, 93, 80],
            borderWidth: 2,
            backgroundColor: 'rgba(11, 79, 255, 0.2)',
            borderColor: '#0b4fff',
            pointBackgroundColor: '#0b4fff'
        }]
    },
    options: {
        responsive: true,
        scales: {
            r: {
                angleLines: { color: '#d0d7ff' },
                grid: { color: '#d0d7ff' },
                pointLabels: { color: '#222' },
                suggestedMin: 0,
                suggestedMax: 100
            }
        }
    }
});
</script>

</body>
</html>
