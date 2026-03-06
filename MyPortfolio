<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sudarshan Yadav — DevOps Engineer</title>
<link href="https://fonts.googleapis.com/css2?family=Clash+Display:wght@400;500;600;700&family=Cabinet+Grotesk:wght@400;500;700&display=swap" rel="stylesheet">
<style>
:root {
  --bg: #050810;
  --surface: #0c1120;
  --surface2: #111827;
  --border: #1e293b;
  --accent: #00d4ff;
  --accent2: #7c3aed;
  --accent3: #f59e0b;
  --text: #f1f5f9;
  --muted: #64748b;
  --green: #10b981;
}

*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

html { scroll-behavior: smooth; }

body {
  background: var(--bg);
  color: var(--text);
  font-family: 'Cabinet Grotesk', sans-serif;
  overflow-x: hidden;
  cursor: none;
}

/* Custom cursor */
.cursor {
  width: 12px; height: 12px;
  background: var(--accent);
  border-radius: 50%;
  position: fixed;
  pointer-events: none;
  z-index: 9999;
  transition: transform 0.1s;
  mix-blend-mode: screen;
}
.cursor-ring {
  width: 36px; height: 36px;
  border: 1px solid rgba(0,212,255,0.4);
  border-radius: 50%;
  position: fixed;
  pointer-events: none;
  z-index: 9998;
  transition: transform 0.15s, left 0.08s, top 0.08s;
}

/* Grid background */
body::before {
  content: '';
  position: fixed;
  inset: 0;
  background-image: 
    linear-gradient(rgba(0,212,255,0.03) 1px, transparent 1px),
    linear-gradient(90deg, rgba(0,212,255,0.03) 1px, transparent 1px);
  background-size: 60px 60px;
  pointer-events: none;
  z-index: 0;
}

/* NAV */
nav {
  position: fixed;
  top: 0; left: 0; right: 0;
  z-index: 100;
  padding: 18px 48px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  backdrop-filter: blur(20px);
  background: rgba(5,8,16,0.8);
  border-bottom: 1px solid var(--border);
}

.nav-logo {
  font-family: 'Clash Display', sans-serif;
  font-size: 1.2rem;
  font-weight: 700;
  color: var(--accent);
  letter-spacing: -0.5px;
}

.nav-links {
  display: flex;
  gap: 32px;
  list-style: none;
}

.nav-links a {
  color: var(--muted);
  text-decoration: none;
  font-size: 0.88rem;
  font-weight: 500;
  letter-spacing: 0.5px;
  text-transform: uppercase;
  transition: color 0.2s;
}
.nav-links a:hover { color: var(--accent); }

/* HERO */
.hero {
  position: relative;
  min-height: 100vh;
  display: flex;
  align-items: center;
  padding: 0 48px;
  z-index: 1;
  overflow: hidden;
}

.hero-glow {
  position: absolute;
  width: 600px; height: 600px;
  background: radial-gradient(circle, rgba(0,212,255,0.12) 0%, transparent 70%);
  top: 50%; left: 50%;
  transform: translate(-50%, -50%);
  animation: pulseGlow 4s ease-in-out infinite;
  pointer-events: none;
}

.hero-glow2 {
  position: absolute;
  width: 400px; height: 400px;
  background: radial-gradient(circle, rgba(124,58,237,0.1) 0%, transparent 70%);
  top: 20%; right: 10%;
  animation: pulseGlow 6s ease-in-out infinite reverse;
  pointer-events: none;
}

@keyframes pulseGlow {
  0%, 100% { transform: translate(-50%, -50%) scale(1); opacity: 1; }
  50% { transform: translate(-50%, -50%) scale(1.1); opacity: 0.7; }
}

.hero-content {
  max-width: 900px;
  position: relative;
  z-index: 2;
}

.hero-tag {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  border: 1px solid rgba(0,212,255,0.3);
  background: rgba(0,212,255,0.05);
  border-radius: 100px;
  padding: 6px 16px;
  font-size: 0.8rem;
  color: var(--accent);
  letter-spacing: 1px;
  text-transform: uppercase;
  margin-bottom: 28px;
  animation: fadeUp 0.8s ease forwards;
  opacity: 0;
}

.hero-tag .dot {
  width: 6px; height: 6px;
  background: var(--green);
  border-radius: 50%;
  animation: blink 1.5s ease-in-out infinite;
}

@keyframes blink { 0%,100%{opacity:1} 50%{opacity:0.3} }

.hero-name {
  font-family: 'Clash Display', sans-serif;
  font-size: clamp(3.5rem, 8vw, 7rem);
  font-weight: 700;
  line-height: 0.95;
  letter-spacing: -3px;
  animation: fadeUp 0.8s 0.1s ease forwards;
  opacity: 0;
}

.hero-name span {
  background: linear-gradient(135deg, var(--accent) 0%, #7c3aed 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.hero-role {
  font-size: clamp(1.2rem, 3vw, 1.8rem);
  color: var(--muted);
  margin-top: 16px;
  font-weight: 500;
  animation: fadeUp 0.8s 0.2s ease forwards;
  opacity: 0;
}

.hero-desc {
  margin-top: 24px;
  color: #94a3b8;
  font-size: 1.05rem;
  line-height: 1.8;
  max-width: 600px;
  animation: fadeUp 0.8s 0.3s ease forwards;
  opacity: 0;
}

.hero-btns {
  display: flex;
  gap: 16px;
  margin-top: 36px;
  flex-wrap: wrap;
  animation: fadeUp 0.8s 0.4s ease forwards;
  opacity: 0;
}

.btn-primary {
  padding: 14px 32px;
  background: var(--accent);
  color: #000;
  border: none;
  border-radius: 8px;
  font-weight: 700;
  font-size: 0.95rem;
  cursor: none;
  text-decoration: none;
  transition: transform 0.2s, box-shadow 0.2s;
  font-family: 'Cabinet Grotesk', sans-serif;
}
.btn-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 12px 40px rgba(0,212,255,0.4);
}

.btn-outline {
  padding: 14px 32px;
  background: transparent;
  color: var(--text);
  border: 1px solid var(--border);
  border-radius: 8px;
  font-weight: 600;
  font-size: 0.95rem;
  cursor: none;
  text-decoration: none;
  transition: border-color 0.2s, color 0.2s;
  font-family: 'Cabinet Grotesk', sans-serif;
}
.btn-outline:hover { border-color: var(--accent); color: var(--accent); }

/* Floating badges */
.hero-badges {
  position: absolute;
  right: 48px;
  top: 50%;
  transform: translateY(-50%);
  display: flex;
  flex-direction: column;
  gap: 12px;
  animation: fadeUp 0.8s 0.5s ease forwards;
  opacity: 0;
}

.badge-float {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: 12px;
  padding: 14px 20px;
  display: flex;
  align-items: center;
  gap: 12px;
  font-size: 0.85rem;
  white-space: nowrap;
  transition: border-color 0.2s, transform 0.2s;
}
.badge-float:hover { border-color: var(--accent); transform: translateX(-4px); }
.badge-float .icon { font-size: 1.4rem; }
.badge-float strong { display: block; font-size: 1rem; color: var(--text); }
.badge-float span { color: var(--muted); font-size: 0.78rem; }

@keyframes fadeUp {
  from { opacity: 0; transform: translateY(24px); }
  to { opacity: 1; transform: translateY(0); }
}

/* SECTIONS */
section {
  position: relative;
  z-index: 1;
  padding: 100px 48px;
  max-width: 1200px;
  margin: 0 auto;
}

.section-label {
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 3px;
  color: var(--accent);
  font-weight: 700;
  margin-bottom: 12px;
}

.section-title {
  font-family: 'Clash Display', sans-serif;
  font-size: clamp(2rem, 4vw, 3.2rem);
  font-weight: 700;
  letter-spacing: -1.5px;
  line-height: 1.1;
  margin-bottom: 48px;
}

/* SKILLS */
.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 20px;
}

.skill-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: 16px;
  padding: 28px;
  transition: border-color 0.3s, transform 0.3s;
  position: relative;
  overflow: hidden;
}

.skill-card::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 2px;
  background: linear-gradient(90deg, var(--accent), var(--accent2));
  transform: scaleX(0);
  transition: transform 0.3s;
}

.skill-card:hover { border-color: rgba(0,212,255,0.3); transform: translateY(-4px); }
.skill-card:hover::before { transform: scaleX(1); }

.skill-category {
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 2px;
  color: var(--accent);
  font-weight: 700;
  margin-bottom: 16px;
}

.skill-icon { font-size: 2rem; margin-bottom: 12px; }

.skill-title {
  font-family: 'Clash Display', sans-serif;
  font-size: 1.2rem;
  font-weight: 600;
  margin-bottom: 12px;
}

.skill-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 12px;
}

.tag {
  background: rgba(0,212,255,0.08);
  border: 1px solid rgba(0,212,255,0.15);
  color: #94a3b8;
  border-radius: 6px;
  padding: 4px 10px;
  font-size: 0.78rem;
  font-weight: 500;
}

/* EXPERIENCE */
.exp-timeline {
  position: relative;
  padding-left: 32px;
}

.exp-timeline::before {
  content: '';
  position: absolute;
  left: 0; top: 8px; bottom: 0;
  width: 1px;
  background: linear-gradient(to bottom, var(--accent), transparent);
}

.exp-item {
  position: relative;
  margin-bottom: 48px;
}

.exp-item::before {
  content: '';
  position: absolute;
  left: -36px; top: 6px;
  width: 10px; height: 10px;
  border-radius: 50%;
  background: var(--accent);
  box-shadow: 0 0 16px var(--accent);
}

.exp-meta {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-wrap: wrap;
  gap: 8px;
  margin-bottom: 8px;
}

.exp-company {
  font-family: 'Clash Display', sans-serif;
  font-size: 1.3rem;
  font-weight: 600;
}

.exp-period {
  background: rgba(245,158,11,0.1);
  border: 1px solid rgba(245,158,11,0.25);
  color: var(--accent3);
  border-radius: 100px;
  padding: 4px 14px;
  font-size: 0.8rem;
  font-weight: 600;
}

.exp-role {
  color: var(--accent);
  font-weight: 600;
  font-size: 0.95rem;
  margin-bottom: 16px;
}

.exp-points {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 10px;
}

.exp-points li {
  color: #94a3b8;
  font-size: 0.92rem;
  line-height: 1.7;
  padding-left: 20px;
  position: relative;
}

.exp-points li::before {
  content: '▸';
  position: absolute;
  left: 0;
  color: var(--accent);
}

/* PROJECT */
.project-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: 20px;
  padding: 36px;
  transition: border-color 0.3s;
  position: relative;
  overflow: hidden;
}

.project-card::after {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(135deg, rgba(0,212,255,0.04) 0%, rgba(124,58,237,0.04) 100%);
  pointer-events: none;
}

.project-card:hover { border-color: rgba(0,212,255,0.4); }

.project-title {
  font-family: 'Clash Display', sans-serif;
  font-size: 1.6rem;
  font-weight: 700;
  margin-bottom: 8px;
  letter-spacing: -0.5px;
}

.project-client {
  color: var(--accent3);
  font-size: 0.85rem;
  font-weight: 600;
  margin-bottom: 20px;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.project-desc {
  color: #94a3b8;
  line-height: 1.75;
  font-size: 0.95rem;
  margin-bottom: 24px;
}

.project-tech {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 20px;
}

.tech-badge {
  background: rgba(124,58,237,0.1);
  border: 1px solid rgba(124,58,237,0.25);
  color: #a78bfa;
  border-radius: 6px;
  padding: 5px 12px;
  font-size: 0.8rem;
  font-weight: 600;
}

.pipeline-visual {
  display: flex;
  align-items: center;
  gap: 0;
  margin: 28px 0;
  overflow-x: auto;
  padding-bottom: 8px;
}

.pipe-step {
  background: var(--surface2);
  border: 1px solid var(--border);
  border-radius: 8px;
  padding: 10px 14px;
  font-size: 0.75rem;
  font-weight: 600;
  color: var(--text);
  white-space: nowrap;
  flex-shrink: 0;
}

.pipe-step.active { 
  border-color: var(--accent); 
  color: var(--accent);
  background: rgba(0,212,255,0.06);
}

.pipe-arrow {
  color: var(--muted);
  font-size: 1rem;
  padding: 0 6px;
  flex-shrink: 0;
}

/* STATS */
.stats-row {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 20px;
  margin-bottom: 60px;
}

.stat-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: 16px;
  padding: 28px 24px;
  text-align: center;
  transition: border-color 0.2s;
}
.stat-card:hover { border-color: var(--accent); }

.stat-num {
  font-family: 'Clash Display', sans-serif;
  font-size: 2.8rem;
  font-weight: 700;
  color: var(--accent);
  line-height: 1;
}

.stat-label {
  color: var(--muted);
  font-size: 0.85rem;
  margin-top: 8px;
  font-weight: 500;
}

/* CONTACT */
.contact-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: 20px;
  padding: 48px;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.contact-card::before {
  content: '';
  position: absolute;
  inset: -1px;
  background: linear-gradient(135deg, rgba(0,212,255,0.2), rgba(124,58,237,0.2));
  border-radius: 20px;
  z-index: -1;
}

.contact-email {
  font-family: 'Clash Display', sans-serif;
  font-size: clamp(1.2rem, 3vw, 2rem);
  font-weight: 700;
  color: var(--accent);
  margin: 20px 0;
}

.contact-links {
  display: flex;
  justify-content: center;
  gap: 16px;
  flex-wrap: wrap;
  margin-top: 28px;
}

.contact-link {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 12px 24px;
  border: 1px solid var(--border);
  border-radius: 10px;
  color: var(--text);
  text-decoration: none;
  font-weight: 600;
  font-size: 0.9rem;
  transition: border-color 0.2s, color 0.2s, transform 0.2s;
  background: var(--bg);
}
.contact-link:hover { border-color: var(--accent); color: var(--accent); transform: translateY(-2px); }

/* FOOTER */
footer {
  text-align: center;
  padding: 32px 48px;
  border-top: 1px solid var(--border);
  color: var(--muted);
  font-size: 0.85rem;
  position: relative;
  z-index: 1;
}

/* SCROLL REVEAL */
.reveal {
  opacity: 0;
  transform: translateY(32px);
  transition: opacity 0.7s ease, transform 0.7s ease;
}
.reveal.visible { opacity: 1; transform: translateY(0); }

@media (max-width: 768px) {
  nav { padding: 16px 24px; }
  .nav-links { display: none; }
  .hero { padding: 100px 24px 60px; }
  .hero-badges { display: none; }
  section { padding: 70px 24px; }
  .hero-name { letter-spacing: -2px; }
  .contact-card { padding: 32px 24px; }
  footer { padding: 24px; }
}
</style>
</head>
<body>

<div class="cursor" id="cursor"></div>
<div class="cursor-ring" id="cursorRing"></div>

<!-- NAV -->
<nav>
  <div class="nav-logo">SY</div>
  <ul class="nav-links">
    <li><a href="#skills">Skills</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#project">Project</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<!-- HERO -->
<div class="hero">
  <div class="hero-glow"></div>
  <div class="hero-glow2"></div>

  <div class="hero-content">
    <div class="hero-tag">
      <span class="dot"></span>
      Available for new opportunities
    </div>
    <h1 class="hero-name">Sudarshan<br><span>Yadav</span></h1>
    <p class="hero-role">DevOps Engineer · AWS · Kubernetes · CI/CD</p>
    <p class="hero-desc">
      2.5 years building and maintaining cloud infrastructure at Accenture. 
      Passionate about automation, containerization, and keeping systems running at 99%+ uptime.
      Based in Pune, India 🇮🇳
    </p>
    <div class="hero-btns">
      <a href="#contact" class="btn-primary">Get In Touch</a>
      <a href="#experience" class="btn-outline">View Experience →</a>
    </div>
  </div>

  <div class="hero-badges">
    <div class="badge-float">
      <span class="icon">☁️</span>
      <div>
        <strong>AWS Certified</strong>
        <span>Cloud Platforms</span>
      </div>
    </div>
    <div class="badge-float">
      <span class="icon">🐳</span>
      <div>
        <strong>Docker & K8s</strong>
        <span>Containerization</span>
      </div>
    </div>
    <div class="badge-float">
      <span class="icon">⚙️</span>
      <div>
        <strong>CI/CD Pipelines</strong>
        <span>Jenkins · GitHub Actions</span>
      </div>
    </div>
    <div class="badge-float">
      <span class="icon">📊</span>
      <div>
        <strong>Monitoring</strong>
        <span>CloudWatch · Grafana</span>
      </div>
    </div>
  </div>
</div>

<!-- STATS -->
<section>
  <div class="stats-row reveal">
    <div class="stat-card">
      <div class="stat-num">2.5</div>
      <div class="stat-label">Years Experience</div>
    </div>
    <div class="stat-card">
      <div class="stat-num">5+</div>
      <div class="stat-label">Enterprise Apps Managed</div>
    </div>
    <div class="stat-card">
      <div class="stat-num">40%</div>
      <div class="stat-label">Manual Effort Reduced</div>
    </div>
    <div class="stat-card">
      <div class="stat-num">99%</div>
      <div class="stat-label">Service Availability</div>
    </div>
    <div class="stat-card">
      <div class="stat-num">20+</div>
      <div class="stat-label">Incidents Resolved</div>
    </div>
  </div>
</section>

<!-- SKILLS -->
<section id="skills">
  <div class="reveal">
    <p class="section-label">What I Work With</p>
    <h2 class="section-title">Technical Skills</h2>
  </div>

  <div class="skills-grid">
    <div class="skill-card reveal">
      <div class="skill-icon">☁️</div>
      <div class="skill-category">Cloud</div>
      <div class="skill-title">AWS Platforms</div>
      <div class="skill-tags">
        <span class="tag">EC2</span><span class="tag">VPC</span><span class="tag">IAM</span>
        <span class="tag">S3</span><span class="tag">RDS</span><span class="tag">ELB</span>
        <span class="tag">Lambda</span><span class="tag">Route53</span>
        <span class="tag">SNS</span><span class="tag">SQS</span>
      </div>
    </div>
    <div class="skill-card reveal">
      <div class="skill-icon">⚙️</div>
      <div class="skill-category">Automation</div>
      <div class="skill-title">CI/CD & IaC</div>
      <div class="skill-tags">
        <span class="tag">Jenkins</span><span class="tag">GitHub Actions</span>
        <span class="tag">Terraform</span><span class="tag">GitOps</span>
        <span class="tag">ArgoCD</span>
      </div>
    </div>
    <div class="skill-card reveal">
      <div class="skill-icon">🐳</div>
      <div class="skill-category">Containers</div>
      <div class="skill-title">Docker & Kubernetes</div>
      <div class="skill-tags">
        <span class="tag">Docker</span><span class="tag">Kubernetes</span>
        <span class="tag">AWS EKS</span><span class="tag">Helm</span>
        <span class="tag">Docker Hub</span>
      </div>
    </div>
    <div class="skill-card reveal">
      <div class="skill-icon">📊</div>
      <div class="skill-category">Observability</div>
      <div class="skill-title">Monitoring & Logging</div>
      <div class="skill-tags">
        <span class="tag">CloudWatch</span><span class="tag">Prometheus</span>
        <span class="tag">Grafana</span>
      </div>
    </div>
    <div class="skill-card reveal">
      <div class="skill-icon">💻</div>
      <div class="skill-category">Systems</div>
      <div class="skill-title">Linux & Scripting</div>
      <div class="skill-tags">
        <span class="tag">Linux</span><span class="tag">Bash</span>
        <span class="tag">Python</span><span class="tag">Shell Scripts</span>
      </div>
    </div>
    <div class="skill-card reveal">
      <div class="skill-icon">🔐</div>
      <div class="skill-category">Security</div>
      <div class="skill-title">DevSecOps</div>
      <div class="skill-tags">
        <span class="tag">IAM Policies</span><span class="tag">Trivy</span>
        <span class="tag">SonarQube</span><span class="tag">Least Privilege</span>
      </div>
    </div>
  </div>
</section>

<!-- EXPERIENCE -->
<section id="experience">
  <div class="reveal">
    <p class="section-label">Where I've Worked</p>
    <h2 class="section-title">Experience</h2>
  </div>

  <div class="exp-timeline reveal">
    <div class="exp-item">
      <div class="exp-meta">
        <div class="exp-company">Accenture Solutions Pvt. Ltd</div>
        <div class="exp-period">Sep 2023 – Present</div>
      </div>
      <div class="exp-role">DevOps Engineer · Pune, India</div>
      <ul class="exp-points">
        <li>Configured and managed AWS resources (EC2, S3, IAM, VPC, RDS) supporting <strong>5+ enterprise applications</strong> across dev and production environments.</li>
        <li>Designed and implemented CI/CD pipelines using Jenkins and GitHub Actions, reducing manual deployment effort by <strong>40%</strong>.</li>
        <li>Monitored cloud infrastructure using Amazon CloudWatch, responding to <strong>20+ production incidents</strong> and maintaining <strong>99%+ service availability</strong>.</li>
        <li>Performed Linux administration across <strong>10+ servers</strong> — user access management, log analysis, package installation, and troubleshooting.</li>
        <li>Implemented IAM roles and policies following <strong>least-privilege principles</strong> for secure access control.</li>
        <li>Developed Shell/Python automation scripts to streamline operational workflows and eliminate repetitive manual tasks.</li>
        <li>Deployed containerized applications on <strong>AWS EKS</strong> using Docker and Kubernetes for scalable, highly available environments.</li>
      </ul>
    </div>
  </div>
</section>

<!-- PROJECT -->
<section id="project">
  <div class="reveal">
    <p class="section-label">What I've Built</p>
    <h2 class="section-title">Featured Project</h2>
  </div>

  <div class="project-card reveal">
    <div class="project-title">Cloud-Native CI/CD Pipeline with Kubernetes & GitOps</div>
    <div class="project-client">Client: CloudBridge Solutions Inc. · Containerized Enterprise Applications</div>

    <p class="project-desc">
      Designed and implemented a complete end-to-end CI/CD pipeline integrated with GitOps principles. 
      Automated the entire lifecycle from code commit to production deployment on AWS EKS with zero-downtime delivery.
    </p>

    <div class="pipeline-visual">
      <div class="pipe-step active">GitHub Push</div>
      <div class="pipe-arrow">→</div>
      <div class="pipe-step active">Jenkins Build</div>
      <div class="pipe-arrow">→</div>
      <div class="pipe-step active">Maven Test</div>
      <div class="pipe-arrow">→</div>
      <div class="pipe-step active">SonarQube</div>
      <div class="pipe-arrow">→</div>
      <div class="pipe-step active">Trivy Scan</div>
      <div class="pipe-arrow">→</div>
      <div class="pipe-step active">Docker Build</div>
      <div class="pipe-arrow">→</div>
      <div class="pipe-step active">Docker Hub</div>
      <div class="pipe-arrow">→</div>
      <div class="pipe-step active">ArgoCD</div>
      <div class="pipe-arrow">→</div>
      <div class="pipe-step active">EKS Deploy</div>
      <div class="pipe-arrow">→</div>
      <div class="pipe-step active">Slack Alert</div>
    </div>

    <ul class="exp-points">
      <li>Built and tested applications using Apache Maven with static code analysis via SonarQube for quality gates.</li>
      <li>Containerized applications using Docker and pushed images to Docker Hub with Trivy security scanning before deployment.</li>
      <li>Implemented GitOps-based continuous deployment using ArgoCD — Kubernetes manifests managed in Git for full auditability.</li>
      <li>Deployed on Amazon EKS with automated rolling updates and <strong>zero downtime deployment</strong>.</li>
      <li>Integrated Slack notifications for real-time pipeline status and deployment alerts.</li>
    </ul>

    <div class="project-tech">
      <span class="tech-badge">AWS EKS</span>
      <span class="tech-badge">Jenkins</span>
      <span class="tech-badge">ArgoCD</span>
      <span class="tech-badge">Docker</span>
      <span class="tech-badge">Kubernetes</span>
      <span class="tech-badge">Terraform</span>
      <span class="tech-badge">SonarQube</span>
      <span class="tech-badge">Trivy</span>
      <span class="tech-badge">Maven</span>
      <span class="tech-badge">GitHub</span>
      <span class="tech-badge">Slack</span>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <div class="reveal">
    <p class="section-label">Let's Connect</p>
    <h2 class="section-title">Get In Touch</h2>
  </div>

  <div class="contact-card reveal">
    <p style="color: var(--muted); font-size: 1rem;">Open to DevOps / Cloud Engineer roles. Let's talk!</p>
    <div class="contact-email">sudarshanyadav4080@gmail.com</div>
    <p style="color: var(--muted); font-size: 0.9rem;">📍 Pune, Maharashtra, India &nbsp;|&nbsp; 📞 +91 7709877817</p>

    <div class="contact-links">
      <a href="mailto:sudarshanyadav4080@gmail.com" class="contact-link">
        ✉️ &nbsp; Email Me
      </a>
      <a href="https://www.linkedin.com/in/sudarshan-yadav/" target="_blank" class="contact-link">
        💼 &nbsp; LinkedIn
      </a>
      <a href="https://github.com/Sudarshanydv" target="_blank" class="contact-link">
        🐙 &nbsp; GitHub
      </a>
    </div>
  </div>
</section>

<footer>
  <p>Designed & built with ❤️ · Sudarshan Yadav · DevOps Engineer · Pune, India · 2025</p>
</footer>

<script>
// Custom cursor
const cursor = document.getElementById('cursor');
const ring = document.getElementById('cursorRing');
let mouseX = 0, mouseY = 0;
let ringX = 0, ringY = 0;

document.addEventListener('mousemove', e => {
  mouseX = e.clientX;
  mouseY = e.clientY;
  cursor.style.left = mouseX - 6 + 'px';
  cursor.style.top = mouseY - 6 + 'px';
});

function animateRing() {
  ringX += (mouseX - ringX - 18) * 0.12;
  ringY += (mouseY - ringY - 18) * 0.12;
  ring.style.left = ringX + 'px';
  ring.style.top = ringY + 'px';
  requestAnimationFrame(animateRing);
}
animateRing();

document.querySelectorAll('a, button').forEach(el => {
  el.addEventListener('mouseenter', () => cursor.style.transform = 'scale(2.5)');
  el.addEventListener('mouseleave', () => cursor.style.transform = 'scale(1)');
});

// Scroll reveal
const reveals = document.querySelectorAll('.reveal');
const observer = new IntersectionObserver(entries => {
  entries.forEach((entry, i) => {
    if (entry.isIntersecting) {
      setTimeout(() => entry.target.classList.add('visible'), i * 80);
    }
  });
}, { threshold: 0.1 });
reveals.forEach(el => observer.observe(el));
</script>
</body>
</html>
