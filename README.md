<h1 align="center">Hi 👋, I'm sumant jena</h1>
<h1 align="center"> ⚙️ DevOps Engineer | 🚀 Automating infrastructure & CI/CD  
☁️ Skilled in AWS | Docker | Kubernetes | Jenkins | Terraform  
🔐 Passionate about Cloud, Security & Scalability  
🤝 Open to collaboration on DevOps & Cloud projects </h1><!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>DevOps Engineer — Animated Profile Card</title>
  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --accent:#00d4ff;
      --accent-2:#7c3aed;
      --muted:#9aa7b2;
      --glass: rgba(255,255,255,0.04);
    }
    *{box-sizing:border-box}
    body{
      margin:0; min-height:100vh; display:grid; place-items:center; font-family:Inter,ui-sans-serif,system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial; background: radial-gradient(1200px 600px at 10% 10%, rgba(124,58,237,0.08), transparent 8%), radial-gradient(1000px 450px at 90% 80%, rgba(0,212,255,0.05), transparent 8%), var(--bg); color:#e6eef3;
    }
    .card{
      width:min(880px,94%); max-width:900px; display:grid; grid-template-columns:260px 1fr; gap:24px; padding:26px; background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); border-radius:18px; box-shadow: 0 8px 30px rgba(2,6,23,0.6); border:1px solid rgba(255,255,255,0.03);
      align-items:center;
    }
    /* left column */
    .profile{
      padding:18px; border-radius:12px; background:var(--card); display:flex; flex-direction:column; gap:14px; align-items:center; position:relative; overflow:visible;
    }
    .avatar{
      width:120px; height:120px; border-radius:50%; background:linear-gradient(135deg,var(--accent),var(--accent-2)); display:grid; place-items:center; font-weight:700; font-size:42px; color:#041125; box-shadow: 0 6px 18px rgba(124,58,237,0.18), inset 0 -6px 18px rgba(255,255,255,0.06);
      border:4px solid rgba(255,255,255,0.06);
    }
    .name{font-size:20px; font-weight:700}
    .role{color:var(--muted); font-size:13px}
    .badges{display:flex; gap:8px; flex-wrap:wrap; justify-content:center}
    .badge{background:var(--glass); padding:6px 10px; border-radius:999px; font-size:12px; color:var(--muted); border:1px solid rgba(255,255,255,0.02)}

    /* animated gears */
    .gears{position:absolute; left:-40px; top:-24px; opacity:0.12}
    .gear svg{width:120px;height:120px; transform-origin:center; animation:spin 8s linear infinite}
    .gear.gear-2 svg{animation-duration:5s; transform-origin:center;}
    @keyframes spin{from{transform:rotate(0)} to{transform:rotate(360deg)}}

    /* right column */
    .content{padding:10px 6px}
    .headline{display:flex; justify-content:space-between; align-items:center}
    .headline h1{margin:0;font-size:18px}
    .links{display:flex; gap:10px}
    .chip{display:inline-flex; gap:8px; align-items:center; padding:8px 12px; border-radius:999px; background:linear-gradient(90deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); border:1px solid rgba(255,255,255,0.03); font-size:13px}

    .about{margin-top:12px; color:var(--muted); line-height:1.45}

    /* skill bars */
    .skills{display:grid; grid-template-columns:repeat(2,1fr); gap:12px; margin-top:16px}
    .skill{display:flex; flex-direction:column; gap:6px}
    .skill .label{display:flex; justify-content:space-between; font-size:13px}
    .bar{height:10px; background:rgba(255,255,255,0.04); border-radius:999px; overflow:hidden}
    .bar > i{display:block; height:100%; width:60%; background:linear-gradient(90deg,var(--accent),var(--accent-2)); border-radius:999px; transform-origin:left; animation:grow 1.1s cubic-bezier(.2,.9,.2,1) both}
    .bar[data-value="90"] > i{width:90%}
    .bar[data-value="80"] > i{width:80%}
    .bar[data-value="75"] > i{width:75%}
    .bar[data-value="70"] > i{width:70%}
    @keyframes grow{from{width:0} to{width:var(--w,60%)}}

    /* pipeline animation */
    .pipeline{margin-top:20px; background:linear-gradient(90deg, rgba(255,255,255,0.01), rgba(255,255,255,0.02)); padding:12px; border-radius:12px; display:flex; gap:8px; align-items:center}
    .stage{display:flex; gap:8px; align-items:center; padding:10px 12px; border-radius:10px; background:rgba(255,255,255,0.02); border:1px solid rgba(255,255,255,0.02)}
    .dot{width:10px;height:10px;border-radius:50%; background:var(--muted); box-shadow:0 0 12px rgba(0,0,0,0.6)}
    .stage.active .dot{background:var(--accent); box-shadow:0 0 10px rgba(0,212,255,0.22); animation:pulse 1.6s ease-in-out infinite}
    @keyframes pulse{0%{transform:scale(1)}50%{transform:scale(1.25)}100%{transform:scale(1)}}

    /* footer */
    .footer{display:flex; gap:8px; margin-top:18px; align-items:center}
    .social a{display:inline-flex; align-items:center; gap:8px; padding:8px 10px; border-radius:8px; text-decoration:none; color:inherit; font-size:13px; border:1px solid rgba(255,255,255,0.03)}

    /* responsive */
    @media (max-width:760px){
      .card{grid-template-columns:1fr; padding:18px}
      .gears{display:none}
    }
  </style>
</head>
<body>
  <main class="card" role="main">
    <div class="profile">
      <!-- decorative gears -->
      <div class="gears" aria-hidden="true">
        <div class="gear gear-1">
          <!-- simple gear svg -->
          <svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
            <g fill="white">
              <path d="M80 55v-10l8-4-6-12-9 2-6-8 2-12-12-2-4 9-10 1-4-9L30 6l-12 6 2 12-6 8-9-2-6 12 8 4v10l-8 4 6 12 9-2 6 8-2 12 12 2 4-9 10-1 4 9 12-6-2-12 6-8 9 2 6-12-8-4zM50 66a16 16 0 1 1 0-32 16 16 0 0 1 0 32z" opacity="0.9"/>
            </g>
          </svg>
        </div>
        <div class="gear gear-2" style="position:relative; left:48px; top:18px; opacity:0.14">
          <svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
            <g fill="white">
              <path d="M73 55v-8l6-3-5-9-6 1-4-6 2-9-9-1-3 7-8 1-3-7-9 1 2 9-4 6-6-1-5 9 6 3v8l-6 3 5 9 6-1 4 6-2 9 9 1 3-7 8-1 3 7 9-1-2-9 4-6 6 1 5-9-6-3zM50 64a14 14 0 1 1 0-28 14 14 0 0 1 0 28z"/>
            </g>
          </svg>
        </div>
      </div>

      <div class="avatar" aria-hidden="false">SJ</div>
      <div class="name">Sumant Jena</div>
      <div class="role">DevOps Engineer — Cloud · CI/CD · Automation</div>
      <div class="badges">
        <div class="badge">AWS</div>
        <div class="badge">Docker</div>
        <div class="badge">Kubernetes</div>
        <div class="badge">Terraform</div>
        <div class="badge">CI/CD</div>
      </div>
    </div>

    <section class="content">
      <div class="headline">
        <h1>Automating infrastructure & delivering reliable pipelines</h1>
        <div class="links">
          <a class="chip" href="#" target="_blank" rel="noopener">GitHub</a>
          <a class="chip" href="#" target="_blank" rel="noopener">LinkedIn</a>
        </div>
      </div>

      <p class="about" id="about">I build cloud-native infrastructure, create repeatable CI/CD pipelines, and automate deployments for scalable systems. I combine networking background (CCNA/CCNP) with DevOps tooling to make systems resilient and observable.</p>

      <div class="skills">
        <div class="skill">
          <div class="label"><span>Infrastructure as Code</span><span>90%</span></div>
          <div class="bar" data-value="90"><i></i></div>
        </div>
        <div class="skill">
          <div class="label"><span>Containerization & Orchestration</span><span>80%</span></div>
          <div class="bar" data-value="80"><i></i></div>
        </div>
        <div class="skill">
          <div class="label"><span>CI/CD & Automation</span><span>75%</span></div>
          <div class="bar" data-value="75"><i></i></div>
        </div>
        <div class="skill">
          <div class="label"><span>Cloud (AWS/GCP)</span><span>70%</span></div>
          <div class="bar" data-value="70"><i></i></div>
        </div>
      </div>

      <div class="pipeline" aria-hidden="false">
        <div class="stage active"><div class="dot"></div><div>Code</div></div>
        <div class="stage"><div class="dot"></div><div>Build</div></div>
        <div class="stage"><div class="dot"></div><div>Test</div></div>
        <div class="stage"><div class="dot"></div><div>Deploy</div></div>
        <div class="stage"><div class="dot"></div><div>Monitor</div></div>
      </div>

      <div class="footer">
        <div class="social">
          <a href="#" target="_blank" rel="noopener">📁 Projects</a>
          <a href="#" target="_blank" rel="noopener">📄 Resume</a>
        </div>
      </div>

    </section>
  </main>

  <script>
    // Simple typing-like highlight for "about" text
    (function(){
      const about = document.getElementById('about');
      const orig = about.textContent;
      // small animation to emphasise keywords
      const keywords = ['cloud-native','CI/CD','automation','resilient','observable'];
      let idx=0;
      setInterval(()=>{
        const k = keywords[idx++ % keywords.length];
        about.innerHTML = orig.replace(new RegExp('('+k+')','i'), '<strong style="color:var(--accent)">$1</strong>');
      }, 2200);

      // animate skill bars from 0 to value on load
      document.querySelectorAll('.bar').forEach(b=>{
        const val = b.getAttribute('data-value') || '60';
        const el = b.querySelector('i');
        el.style.width='0%';
        setTimeout(()=>{ el.style.width = val + '%'; }, 120);
      });

      // cycle pipeline active stage
      const stages = document.querySelectorAll('.pipeline .stage');
      let s=0;
      setInterval(()=>{
        stages.forEach(st=>st.classList.remove('active'));
        stages[s % stages.length].classList.add('active');
        s++;
      }, 1800);
    })();
  </script>
</body>
</html>


<h3 align="center">A passionate frontend developer from India</h3>

<p align="left"> <img src="https://komarev.com/ghpvc/?username=sumantjena05-crypto&label=Profile%20views&color=0e75b6&style=flat" alt="sumantjena05-crypto" /> </p>

<p align="left"> <a href="https://github.com/ryo-ma/github-profile-trophy"><img src="https://github-profile-trophy.vercel.app/?username=sumantjena05-crypto" alt="sumantjena05-crypto" /></a> </p>

- 🔭 I’m currently working on **movie ticket BOOKING SYSTEM**

- 🌱 I’m currently learning **python oracle HTML CSS JAVASCRIPT DJANGO**

- 📫 How to reach me **sumantjena05@gmail.com**

<h3 align="left">Connect with me:</h3>
<p align="left">
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://aws.amazon.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.djangoproject.com/" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/django.svg" alt="django" width="40" height="40"/> </a> <a href="https://www.docker.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/> </a> <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://www.jenkins.io" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/jenkins/jenkins-icon.svg" alt="jenkins" width="40" height="40"/> </a> <a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> <a href="https://www.mongodb.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="mongodb" width="40" height="40"/> </a> <a href="https://www.oracle.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/oracle/oracle-original.svg" alt="oracle" width="40" height="40"/> </a> <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> </p>

<p><img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=sumantjena05-crypto&show_icons=true&locale=en&layout=compact" alt="sumantjena05-crypto" /></p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=sumantjena05-crypto&show_icons=true&locale=en" alt="sumantjena05-crypto" /></p>

<p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=sumantjena05-crypto&" alt="sumantjena05-crypto" /></p>
