-->
<div class="contrib-dot bg-emerald-400"></div>
<div class="contrib-dot bg-emerald-500"></div>
<div class="contrib-dot bg-emerald-600"></div>
<div class="contrib-dot bg-emerald-700"></div>
</div>
</div>
<!-- ... -->
</div>
</div>
</div>


</section>
</main>


<!-- Footer -->
<footer class="mt-8 text-center text-slate-400">
<small>Made with ♥ • Customizable GitHub-style dashboard for DevOps engineers</small>
</footer>
</div>


<script>
// Simple demo script to make the dashboard interactive.
const state = {
name: 'Abhay Agarwal',
role: 'DevOps Engineer • CI/CD • Kubernetes • Terraform',
avatar: 'https://avatars.githubusercontent.com/u/9919?s=200&v=4',
repoCount: 42,
starCount: '1.2k',
followerCount: 876,
github: 'https://github.com/yourusername'
}


document.getElementById('name').innerText = state.name
document.getElementById('role').innerText = state.role
document.getElementById('avatar').src = state.avatar
document.getElementById('repoCount').innerText = state.repoCount
document.getElementById('starCount').innerText = state.starCount
document.getElementById('followerCount').innerText = state.followerCount
document.getElementById('githubLink').href = state.github
document.getElementById('resumeBtn').href = '/resume.pdf'


// Theme toggle
const themeBtn = document.getElementById('themeToggle')
themeBtn.addEventListener('click', () => {
const isDark = document.documentElement.classList.toggle('light')
if (isDark) {
document.body.classList.remove('bg-gradient-to-b', 'from-slate-900', 'via-slate-900', 'to-slate-800')
document.body.style.background = 'linear-gradient(180deg, #f8fafc, #eef2ff)'
document.body.style.color = '#0f172a'
themeBtn.innerText = '☀️'
} else {
document.body.style.background = ''
document.body.style.color = ''
themeBtn.innerText = '🌙'
}
})


// Small responsive tweak for demo
window.addEventListener('resize', () => {
// future enhancements: fetch GitHub data, load charts, etc.
})


</script>
</body>
</html>
