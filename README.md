<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Meet the Team</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header>
    <h1>About Us</h1>
    <p>We are a team of passionate developers building modern web applications.</p>
  </header>

  <section class="team">
    <div class="card">
      <img src="https://via.placeholder.com/150" alt="Team Member 1" />
      <h2>Alice Smith</h2>
      <p>Frontend Developer</p>
    </div>

    <div class="card">
      <img src="https://via.placeholder.com/150" alt="Team Member 2" />
      <h2>Bob Johnson</h2>
      <p>Backend Developer</p>
    </div>

    <div class="card">
      <img src="https://via.placeholder.com/150" alt="Team Member 3" />
      <h2>Carol Lee</h2>
      <p>UI/UX Designer</p>
    </div>
  </section>
</body>
</html>

/* Basic reset and styles */
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background: #f7f7f7;
  color: #333;
}

header {
  text-align: center;
  padding: 2rem 1rem;
  background-color: #4CAF50;
  color: white;
}

.team {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 1.5rem;
  padding: 2rem;
}

.card {
  background: white;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  text-align: center;
  width: 250px;
  transition: transform 0.3s, box-shadow 0.3s;
  padding: 1rem;
}

.card img {
  border-radius: 50%;
  width: 150px;
  height: 150px;
  object-fit: cover;
}

.card h2 {
  margin: 1rem 0 0.5rem;
}

.card p {
  color: #777;
  font-size: 0.95rem;
}

/* Hover effect */
.card:hover {
  transform: translateY(-10px);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}

/* Responsive layout */
@media (max-width: 768px) {
  .team {
    flex-direction: column;
    align-items: center;
  }
}

<script>
  function showInfo(card) {
    const name = card.getAttribute("data-name");
    const role = card.getAttribute("data-role");
    alert(${name} - ${role});
  }
</script>
