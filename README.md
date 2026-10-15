
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SAFESCAPE 360°</title>
<style>
body{margin:0;font-family:Arial,sans-serif;background:#f1f8f6;color:#183b3b;line-height:1.6}
header,footer{background:#103b3b;color:white;text-align:center;padding:22px}
header h1{margin:0}
.hero{text-align:center;padding:45px 18px;background:#d9f1e8}
.hero h2{font-size:29px}
.button,button{background:#087f70;color:white;padding:12px 18px;border:0;border-radius:7px;text-decoration:none;font-weight:bold;cursor:pointer}
section{max-width:800px;margin:auto;padding:20px}
.card{background:white;padding:20px;margin:15px 0;border-radius:12px;box-shadow:0 3px 12px #00000010}
h2,h3{color:#12665b}
label{display:block;margin-top:12px;font-weight:bold}
input,select,textarea{width:100%;padding:11px;margin-top:5px;border:1px solid #b8cfca;border-radius:7px;font:inherit;box-sizing:border-box}
.note{font-size:13px;color:#536765}
</style>
</head>
<body>

<header>
<h1>SAFESCAPE 360°</h1>
<p>Surakshit • Saksham • Samriddh</p>
</header>

<div class="hero">
<h2>Safer Streets. Stronger Communities.</h2>
<p>Promoting women's safety and safer public spaces for everyone.</p>
<a class="button" href="#report">Report a Safety Concern</a>
</div>

<section>
<div class="card">
<h2>Our Mission</h2>
<p>We encourage communities to identify public-space safety concerns and promote practical solutions such as better lighting, visible safety signs and accessible pathways.</p>
</div>
<h2>Our Proposed Solutions</h2>
<div class="card"><h3>💡 Better Lighting</h3><p>Promote well-lit streets, pathways and public transport stops.</p></div>
<div class="card"><h3>🪧 Public Safety Signage</h3><p>Encourage visible emergency helpline information and directions to help.</p></div>
<div class="card"><h3>🤝 Community Participation</h3><p>Support collaboration between residents and local authorities.</p></div>
</section>

<section id="report">
<div class="card">
<h2>Report a Public Space Safety Issue</h2>
<p>Use this form to demonstrate how a public-space concern could be reported.</p>

<form id="reportForm">
<label for="category">Concern Category</label>
<select id="category" required>
<option value="">Choose a category</option>
<option>Poor street lighting</option>
<option>Need for public safety signage</option>
<option>Unsafe pathway</option>
<option>Public transport stop safety</option>
<option>Other concern</option>
</select>

<label for="area">General Area</label>
<input id="area" placeholder="e.g. Public bus stop near college" required>

<label for="details">Describe the Concern</label>
<textarea id="details" rows="4" placeholder="Describe the issue and possible improvement" required></textarea>

<button type="submit">Submit Demo Report</button>
<p id="message" role="status"></p>
</form>

<p class="note">Demo only: this form does not send reports to police or authorities and does not save them to a database. Do not enter personal or sensitive information.</p>
</div>
</section>

<footer>
<p>SAFESCAPE 360°</p>
<p>Surakshit • Saksham • Samriddh</p>
<p>Safer public spaces begin with community action.</p>
</footer>

<script>
document.getElementById("reportForm").addEventListener("submit",function(event){
event.preventDefault();
document.getElementById("message").textContent="Demo report submitted successfully! Thank you for supporting safer public spaces.";
this.reset();
});
</script>

</body>
</html>

