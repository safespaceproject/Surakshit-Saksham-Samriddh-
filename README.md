
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SAFESCAPE 360° | Safer Public Spaces</title>
  <style>
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f3f8f7;
      color: #183b3b;
      line-height: 1.6;
    }
    header {
      background: #103b3b;
      color: white;
      padding: 22px 18px;
      text-align: center;
    }
    header h1 { margin: 0; font-size: 28px; }
    header p { margin: 6px 0 0; color: #c8e9df; }
    nav {
      padding: 12px;
      text-align: center;
      background: #ffffff;
    }
    nav a {
      color: #176b61;
      text-decoration: none;
      margin: 0 10px;
      font-weight: bold;
    }
    .hero {
      padding: 48px 20px;
      text-align: center;
      background: linear-gradient(135deg, #d8f1e8, #edf7fb);
    }
    .hero h2 { font-size: 32px; margin: 0 0 12px; }
    .hero p { max-width: 600px; margin: 0 auto 22px; }
    .button {
      display: inline-block;
      background: #087f70;
      color: white;
      padding: 12px 22px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
    }
    section { padding: 28px 18px; max-width: 850px; margin: auto; }
    .card {
      background: white;
      padding: 20px;
      margin: 14px 0;
      border-radius: 12px;
      box-shadow: 0 3px 12px #183b3b12;
    }
    h2, h3 { color: #12665b; }
    label { display: block; margin-top: 12px; font-weight: bold; }
    input, select, textarea {
      width: 100%;
      padding: 11px;
      margin-top: 5px;
      border: 1px solid #b8cfca;
      border-radius: 7px;
      font: inherit;
    }
    button {
      margin-top: 16px;
      padding: 12px 18px;
      background: #087f70;
      color: white;
      border: 0;
      border-radius: 7px;
      font-size: 16px;
      font-weight: bold;
    }
    #message { color: #12665b; font-weight: bold; }
    footer {
      text-align: center;
      padding: 22px;
      background: #103b3b;
      color: white;
    }
    .note { font-size: 14px; color: #526765; }
  </style>
</head>
<body>

<header>
  <h1>SAFESCAPE 360°</h1>
  <p>Surakshit • Saksham • Samriddh</p>
</header>

<nav>
  <a href="#about">About</a>
  <a href="#solutions">Solutions</a>
  <a href="#report">Demo Report</a>
</nav>

<div class="hero">
  <h2>Safer Streets. Stronger Communities.</h2>
  <p>
    A community initiative promoting women's safety
    and safer, more accessible public spaces for everyone.
  </p>
  <a class="button" href="#report">Report a Safety Concern</a>
</div>

<section id="about">
  <div class="card">
    <h2>Our Mission</h2>
    <p>
      SAFESCAPE 360° aims to encourage communities to identify
      public-space safety concerns and support practical solutions
      such as better lighting, visible help signs and accessible routes.
    </p>
  </div>
</section>

<section id="solutions">
  <h2>Our Proposed Solutions</h2>
  <div class="card">
    <h3>💡 Better Lighting</h3>
    <p>Encourage well-lit streets, pathways and public transport stops.</p>
  </div>
  <div class="card">
    <h3>🪧 Public Safety Signage</h3>
    <p>Promote visible emergency helpline information and directions to assistance.</p>
  </div>
  <div class="card">
    <h3>🤝 Community Participation</h3>
    <p>Encourage residents and local authorities to work together for safer spaces.</p>
  </div>
</section>

<section id="report">
  <div class="card">
    <h2>Demo Safety Report</h2>
    <p>Describe a public-space concern for this website demonstration.</p>

    <form id="reportForm">
      <label for="category">Concern Category</label>
      <select id="category" required>
        <option value="">Choose a category</option>
        <option>Poor street lighting</option>
        <option>Need for public safety signage</option>
        <option>Unsafe or inaccessible pathway</option>
        <option>Public transport stop safety</option>
        <option>Other public-space concern</option>
      </select>

      <label for="area">General Area (no exact home address)</label>
      <input id="area" type="text" placeholder="e.g. Public bus stop near college" required>

      <label for="details">Describe the Concern</label>
      <textarea id="details" rows="4" placeholder="Explain the issue and a possible improvement..." required></textarea>

      <button type="submit">Submit Demo Report</button>
      <p id="message" role="status"></p>
    </form>
    <p class="note">
      Demonstration only: reports are not sent to authorities or saved to a database.
      Do not enter personal or sensitive information.
    </p>
  </div>
</section>

<footer>
  <p>SAFESCAPE 360°</p>
  <p>Surakshit • Saksham • Samriddh</p>
  <p>Safer public spaces begin with community action.</p>
</footer>

<script>
  document.getElementById("reportForm").addEventListener("submit", function(event) {
    event.preventDefault();
    document.getElementById("message").textContent =
      "Demo report submitted successfully! Thank you for supporting safer public spaces.";
    this.reset();
  });
</script>

</body>
</html>
