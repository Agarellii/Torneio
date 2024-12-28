<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Torneio ABDPS - Standoff 2</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: url('https://via.placeholder.com/1920x1080') no-repeat center center fixed;
      background-size: cover;
      color: white;
      text-align: center;
    }
    .container {
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
      background-color: rgba(0, 0, 0, 0.8);
      border-radius: 10px;
    }
    h1, h2, h3 {
      margin: 10px 0;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 20px 0;
    }
    table, th, td {
      border: 1px solid white;
    }
    th, td {
      padding: 10px;
      text-align: center;
    }
    th {
      background-color: #333;
    }
    input, button {
      padding: 10px;
      margin: 10px 0;
      border: none;
      border-radius: 5px;
    }
    button {
      background-color: #4CAF50;
      color: white;
      cursor: pointer;
    }
    button:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>ABDPS - Torneio Standoff 2</h1>
    <h2>O torneio começará em breve!</h2>
    <p>Inscreva-se e participe do torneio do nosso clã!</p>

    <!-- Formulário para inscrições -->
    <h3>Inscreva-se</h3>
    <form id="form">
      <input type="text" id="name" placeholder="Seu nome" required>
      <button type="submit">Enviar</button>
    </form>

    <!-- Lista de participantes -->
    <h3>Participantes</h3>
    <ul id="participants"></ul>

    <!-- Tabela de organização -->
    <h3>Tabela de Organização do Torneio</h3>
    <h4>Fase 1: Free for All (FFA)</h4>
    <table>
      <thead>
        <tr>
          <th>Rodada</th>
          <th>Mapa</th>
          <th>Vencedor</th>
          <th>Pontos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Rodada 1</td>
          <td>Rust</td>
          <td>—</td>
          <td>—</td>
        </tr>
        <tr>
          <td>Rodada 2</td>
          <td>Sandstone</td>
          <td>—</td>
          <td>—</td>
        </tr>
        <tr>
          <td>Rodada 3</td>
          <td>Province</td>
          <td>—</td>
          <td>—</td>
        </tr>
        <tr>
          <td>Rodada 4</td>
          <td>Zone 9</td>
          <td>—</td>
          <td>—</td>
        </tr>
      </tbody>
    </table>

    <h4>Fase 2: Semi-Finais (1v1)</h4>
    <table>
      <thead>
        <tr>
          <th>Partida</th>
          <th>Mapa</th>
          <th>Participantes</th>
          <th>Vencedor</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Semi-Final 1 (1º vs 4º)</td>
          <td>—</td>
          <td>—</td>
          <td>—</td>
        </tr>
        <tr>
          <td>Semi-Final 2 (2º vs 3º)</td>
          <td>—</td>
          <td>—</td>
          <td>—</td>
        </tr>
      </tbody>
    </table>

    <h4>Fase 3: Final (1v1)</h4>
    <table>
      <thead>
        <tr>
          <th>Partida</th>
          <th>Mapa</th>
          <th>Participantes</th>
          <th>Vencedor</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Final (Vencedores)</td>
          <td>—</td>
          <td>—</td>
          <td>—</td>
        </tr>
      </tbody>
    </table>
  </div>

  <script>
    const form = document.getElementById('form');
    const participantsList = document.getElementById('participants');

    // Lista de participantes
    const participants = [];

    // Adicionar participante
    form.addEventListener('submit', (e) => {
      e.preventDefault();
      const name = document.getElementById('name').value;
      if (name) {
        participants.push(name);
        const li = document.createElement('li');
        li.textContent = name;
        participantsList.appendChild(li);
        document.getElementById('name').value = '';
      }
    });
  </script>
</body>
</html>
