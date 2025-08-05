
 * {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: 'Segoe UI', sans-serif;
  background: linear-gradient(to right, #ECF0F1, #f7f9fa);
  color: #2C3E50;
  padding: 20px;
}

nav {
  display: flex;
  justify-content: space-between;
  background-color: #2C3E50;
  color: white;
  padding: 15px 25px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

nav h2 {
  font-size: 24px;
}

nav a {
  color: white;
  margin-left: 20px;
  text-decoration: none;
  font-weight: bold;
  transition: color 0.3s ease;
}

nav a:hover {
  color: #E67E22;
}

.container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 25px;
  margin-top: 30px;
}

.card {
  background-color: white;
  padding: 25px;
  border-radius: 15px;
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.05);
  transition: transform 0.2s ease;
}

.card:hover {
  transform: translateY(-4px);
}

h3 {
  color: #2C3E50;
  margin-bottom: 15px;
  font-size: 20px;
}

form input,
form select,
form button {
  width: 100%;
  padding: 12px;
  margin-bottom: 12px;
  border: 1px solid #bdc3c7;
  border-radius: 8px;
  font-size: 14px;
  transition: border 0.3s ease;
}

form input:focus {
  border-color: #E67E22;
  outline: none;
}

form button {
  background-color: #E67E22;
  color: white;
  font-weight: bold;
  border: none;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

form button:hover {
  background-color: #cf711b;
}

.todo input,
.gallery input {
  width: 70%;
  padding: 10px;
  border-radius: 6px;
  border: 1px solid #bdc3c7;
}

.todo button,
.gallery button {
  padding: 10px 15px;
  background-color: #2C3E50;
  color: white;
  border: none;
  border-radius: 6px;
  margin-left: 10px;
  cursor: pointer;
  font-weight: bold;
  transition: background-color 0.3s ease;
}

.todo button:hover,
.gallery button:hover {
  background-color: #1a252f;
}

.todo ul,
.gallery .images {
  list-style: none;
  margin-top: 15px;
  padding: 0;
}

.todo li,
.gallery .img-box {
  background-color: #ecf0f1;
  padding: 12px;
  margin-bottom: 10px;
  border-radius: 8px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.gallery .img-box img {
  max-width: 100px;
  height: auto;
  margin-right: 10px;
  border-radius: 6px;
  border: 1px solid #ccc;
}

li button,
.img-box button {
  background: none;
  border: none;
  font-size: 18px;
  color: #e74c3c;
  cursor: pointer;
}

#formMsg {
  font-weight: bold;
  margin-top: 5px;
  font-size: 14px;
}

@media(max-width: 768px) {
  nav {
    flex-direction: column;
    align-items: flex-start;
  }

  nav a {
    margin: 10px 0 0;
  }

  .todo input,
  .gallery input {
    width: 100%;
    margin-bottom: 10px;
  }

  .todo button,
  .gallery button {
    width: 100%;
  }
}
