<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Webpage</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <nav class="navbar">
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>

  <div class="container">
    <main>
      <h2>My Website</h2>
      <p>welcome to my website</p>
    </main>

    <aside class="sidebar">
      <h3>Sidebar Title</h3>
      <p>Here's some extra information or links in the sidebar.</p>
    </aside>
  </div>
  <footer>
    <p>&copy; All rights reserved.</p>
  </footer>
</body>
</html>
#style.css
/* General Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Arial', sans-serif;
    text-decoration: none;
    list-style: none;
    color: #333;
    transition: all 0.3s ease;
    scroll-behavior: smooth;
    font-size: 16px;
}
    
  
  body {
    font-family: 'Arial', sans-serif;
    line-height: 1.6;
    background-color: #f4f4f4;
    color: #333;
    padding: 20px;
    font-size: 16px;
    max-width: 1200px;
  }
  
  /* Header and Navigation Bar */
  header {
    background-color: #af1579;
    color: white;
    padding: 10px 0;
    text-align: center;
    font-size: 2rem;
    font-weight: bold;
    margin-bottom: 20px;
  }
  
  .navbar ul {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    justify-items: center;
    list-style: none;
  }
  
  .navbar li {
    margin: 10px;
  }
  
  .navbar a {
    text-decoration: none;
    color: white;
    font-size: 1.2rem;
    padding: 8px 16px;
  }
  
  .navbar a:hover {
    background-color: #575757;
    border-radius: 4px;
  }
  
  /* Container (Main Layout) */
  .container {
    display: flex;
    justify-content: space-between;
    gap: 20px;
    margin: 20px;
  }
  
  /* Main Content Styling */
  main {
    flex: 3;
    background-color: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  
  main h2 {
    font-size: 1.8rem;
    margin-bottom: 10px;
  }
  
  main p {
    font-size: 1rem;
    margin-bottom: 15px;
  }
  
  main img {
    max-width: 100%;
    border-radius: 8px;
    display: block;
    margin-top: 20px;
  }
  
  /* Sidebar Styling */
  .sidebar {
    flex: 1;
    background-color: #f0f0f0;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  
  .sidebar h3 {
    font-size: 1.5rem;
    margin-bottom: 10px;
  }
  
  .sidebar p {
    font-size: 1rem;
    color: #555;
  }
  
  /* Footer Styling */
  footer {
    text-align: center;
    padding: 20px;
    background-color: #d8cbcb;
    color: white;
    margin-top: 20px;
    font-size: 0.9rem;
  }
  
  /* Media Queries for Responsiveness */
  
  /* Tablet and below (max-width: 768px) */
  @media (max-width: 768px) {
    .navbar ul {
      grid-template-columns: repeat(2, 1fr);
    }
  
    .container {
      flex-direction: column;
      align-items: center;
    }
  
    .sidebar {
      width: 100%;
      margin-top: 20px;
    }
  }
  
  /* Mobile Devices (max-width: 480px) */
  @media (max-width: 480px) {
    .navbar ul {
      grid-template-columns: 1fr;
    }
  
    .navbar a {
      font-size: 1rem;
    }
  
    .container {
      margin: 10px;
    }
  
    .main {
      padding: 10px;
    }
  }
  
