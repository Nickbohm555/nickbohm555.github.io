---
layout: page
title: Nicholas Bohm
---

<style>
body {
  background: radial-gradient(circle at top, #0d0d0d, #000000 70%);
  color: #e0e0e0;
  font-family: "Inter", "Segoe UI", sans-serif;
  text-align: center;
  margin: 0;
  padding: 0;
}

h2 {
  font-size: 2em;
  margin-bottom: 0.4em;
  background: linear-gradient(90deg, #00eaff, #9a5fff);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

p {
  font-size: 1.1em;
  line-height: 1.6em;
  color: #bfbfbf;
  max-width: 750px;
  margin: 0 auto;
}

a {
  color: #00eaff;
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: all 0.2s ease-in-out;
}
a:hover { border-bottom: 1px solid #00eaff; }

/* Tabs */
.tabs {
  display: flex;
  justify-content: center;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
  margin-bottom: 30px;
  padding-top: 20px;
}
.tab {
  padding: 12px 25px;
  cursor: pointer;
  font-weight: 600;
  letter-spacing: 0.5px;
  color: #888;
  border-bottom: 3px solid transparent;
  transition: all 0.3s;
  text-transform: uppercase;
}
.tab:hover { color: #00eaff; }
.tab.active {
  border-color: #00eaff;
  color: #fff;
  text-shadow: 0 0 10px #00eaff;
}
.tab-content {
  display: none;
  animation: fadeIn 0.5s ease;
  padding: 0 20px;
}
.tab-content.active { display: block; }

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}

/* Timeline */
.timeline {
  position: relative;
  max-width: 800px;
  margin: 40px auto;
  padding-left: 20px;
  border-left: 2px solid #00eaff33;
}
.timeline-item {
  margin: 30px 0;
  position: relative;
}
.timeline-item::before {
  content: "";
  position: absolute;
  left: -10px;
  top: 5px;
  width: 16px;
  height: 16px;
  background: linear-gradient(90deg, #00eaff, #9a5fff);
  border-radius: 50%;
  box-shadow: 0 0 10px #00eaff;
}
.timeline-item h3 {
  margin: 0;
  color: #fff;
  font-size: 1.3em;
}
.timeline-item span {
  color: #999;
  font-size: 0.95em;
}
.timeline-item p {
  color: #bfbfbf;
  margin-top: 6px;
  text-align: left;
  max-width: 700px;
}

/* Blog Cards */
.blog-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 20px;
  max-width: 900px;
  margin: 40px auto;
}
.blog-card {
  background: rgba(255,255,255,0.05);
  border: 1px solid rgba(255,255,255,0.1);
  padding: 20px;
  border-radius: 12px;
  transition: all 0.3s ease;
}
.blog-card:hover {
  transform: translateY(-5px);
  border-color: #00eaff;
  box-shadow: 0 0 10px #00eaff55;
}
.blog-card h4 {
  color: #fff;
  margin-bottom: 10px;
}
.blog-card p { font-size: 0.95em; }

/* Image Styling */
.photo {
  border-radius: 12px;
  box-shadow: 0 0 15px #00eaff33;
  margin: 20px auto;
  max-width: 90%;
  transition: transform 0.3s ease;
}
.photo:hover { transform: scale(1.02); }
</style>

<div class="tabs">
  <div class="tab active" data-tab="work">Work History</div>
  <div class="tab" data-tab="tech">Tech Interests</div>
  <div class="tab" data-tab="hobbies">Hobbies</div>
  <div class="tab" data-tab="blog">Blog Posts</div>
</div>

<!-- Work History -->
<div id="work" class="tab-content active">
  <h2>Work History</h2>
  <img src="/assets/profile.jpg" alt="Profile Photo" class="photo" style="max-width:140px;border-radius:50%;">
  <div class="timeline">
    <div class="timeline-item">
      <h3>PricewaterhouseCoopers (PwC) | AI Engineer</h3>
      <span>Dec 2024 – Present | New York, NY</span>
      <p>Developing production microservices in <strong>FastAPI</strong>, <strong>Docker</strong>, and <strong>PostgreSQL</strong> to support scalable enterprise applications. 
      Designed modular backend architectures using <strong>LangGraph</strong> and <strong>LangChain</strong> for dynamic data retrieval, context rehydration, and API generation. 
      Focused on <strong>multi-tenant backend design</strong>, <strong>JWT authentication</strong>, and <strong>Redis</strong>-based persistence for agent workflows.</p>
    </div>

    <div class="timeline-item">
      <h3>Cisco Systems | Software Engineer Intern</h3>
      <span>Jun – Aug 2022 | San Francisco, CA</span>
      <p>Developed <strong>Python</strong> microservices orchestrating large-scale IoT device deployments with <strong>Docker</strong> and internal APIs. 
      Integrated RESTful 5G endpoints that reduced deployment cycles by 40% and improved system reliability by 15%.</p>
    </div>

    <div class="timeline-item">
      <h3>Columbia University</h3>
      <span>BS Computer Science – Application Track | May 2024</span>
      <p>Took a wide variety of classes. Interned at multiple NYC startups as well.</p>
    </div>

    <div class="timeline-item">
      <h3>Colorado College</h3>
      <span>BA Computer Science | May 2022</span>
      <p>Played <strong>D3 Tennis</strong> for the Colorado College team while completing foundational CS courses before transferring to Columbia.</p>
    </div>
  </div>
</div>

<!-- Tech Interests -->
<div id="tech" class="tab-content">
  <h2>Tech Interests</h2>
  <p>
    Currently focused on <strong>agentic systems</strong> and <strong>algorithmic problem solving</strong>.  
    Active on 
    <a href="https://leetcode.com/u/nickbohm555/" target="_blank">LeetCode</a> and 
    <a href="https://codeforces.com/profile/nickbohm555" target="_blank">Codeforces</a>, 
    aiming for the <strong>top 1%</strong> globally.  
    Exploring <strong>LangGraph</strong>’s internals — sub-agent orchestration, dynamic toolkits, and memory persistence — to master agentic AI development end-to-end.
  </p>
</div>

<!-- Hobbies -->
<div id="hobbies" class="tab-content">
  <h2>Hobbies</h2>
  <img src="/assets/sailing.jpg" alt="Sailing on Hudson River" class="photo">
  <p>
    Outside of work, I’m passionate about <strong>lifting and fitness</strong>, improving my <strong>Japanese</strong>, and <strong>traveling</strong> — having visited 
    <strong>33 countries across 5 continents</strong>.  
    I also enjoy <strong>tennis</strong> (former D3 player at Colorado College, though harder to play in NYC) and 
    <strong>sailing on the Hudson River</strong>.
  </p>
</div>

<!-- Blog Posts -->
<div id="blog" class="tab-content">
  <h2>Blog Posts</h2>
  <div class="blog-grid">
    <div class="blog-card">
      <h4>Building Reliable Agentic Systems</h4>
      <p>How modular design and state persistence patterns improve LangGraph-based agent orchestration.</p>
      <a href="#">Read more →</a>
    </div>
    <div class="blog-card">
      <h4>FastAPI Microservices at Scale</h4>
      <p>Design lessons from developing containerized APIs with Postgres, Redis, and distributed task queues.</p>
      <a href="#">Read more →</a>
    </div>
    <div class="blog-card">
      <h4>Optimizing Async Workflows</h4>
      <p>Thread-safe patterns for parallel sub-agent execution and reducing latency in complex pipelines.</p>
      <a href="#">Read more →</a>
    </div>
  </div>
</div>

<script>
const tabs = document.querySelectorAll(".tab");
const contents = document.querySelectorAll(".tab-content");

tabs.forEach(tab => {
  tab.addEventListener("click", () => {
    tabs.forEach(t => t.classList.remove("active"));
    contents.forEach(c => c.classList.remove("active"));
    tab.classList.add("active");
    document.getElementById(tab.dataset.tab).classList.add("active");
  });
});
</script>
