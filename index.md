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
a:hover {
  border-bottom: 1px solid #00eaff;
}

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

.tab:hover {
  color: #00eaff;
}

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

.tab-content.active {
  display: block;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}
</style>

<div class="tabs">
  <div class="tab active" data-tab="work">Current Work</div>
  <div class="tab" data-tab="tech">Tech Interests</div>
  <div class="tab" data-tab="hobbies">Hobbies</div>
</div>

<div id="work" class="tab-content active">
  <h2>Current Work</h2>
  <p>
    I’m currently working on one of PwC’s leading AI initiatives, where I design containerized
    <strong>FastAPI</strong> + <strong>LangGraph</strong> microservices to automate risk analysis and compliance workflows.
    My focus is on building scalable agentic systems that connect structured data, retrieval pipelines, and
    <strong>LangChain</strong> sub-agents for enterprise-grade performance.
  </p>
</div>

<div id="tech" class="tab-content">
  <h2>Tech Interests</h2>
  <p>
    I’m currently working on <strong>agentic systems</strong> and <strong>algorithmic problem solving</strong>.
    I enjoy practicing on
    <a href="https://leetcode.com/u/nickbohm555/" target="_blank">LeetCode</a> and
    <a href="https://codeforces.com/profile/nickbohm555" target="_blank">Codeforces</a>,
    aiming to reach the <strong>top 1%</strong> globally on LeetCode.
    My next goal is to deepen my understanding of the <strong>LangGraph ecosystem</strong> — particularly sub-agent orchestration, dynamic toolkits, and memory persistence.
  </p>
</div>

<div id="hobbies" class="tab-content">
  <h2>Hobbies</h2>
  <p>
    Outside of work, I’m passionate about <strong>lifting and fitness</strong>,
    improving my <strong>Japanese</strong>, and <strong>traveling</strong> — having visited
    <strong>33 countries across 5 continents</strong>. 
    I also love <strong>sailing on the Hudson River</strong>.
  </p>
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
