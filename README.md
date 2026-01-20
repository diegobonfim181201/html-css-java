
│
├── index.html
├── login.html
├── dashboard.html
├── accounts.html
├── cards.html
├── pix.html
├── transactions.html
├── loans.html
├── investments.html
├── support.html
├── profile.html
│
├── css/
│   └── style.css
│
├── js/
│   ├── api.js
│   ├── auth.js
│   ├── dashboard.js
│   ├── accounts.js
│   ├── cards.js
│   ├── pix.js
│   ├── transactions.js
│   ├── loans.js
│   ├── investments.js
│   └── support.js
│
└── assets/
    └── logo.png
✅ 1️⃣ index.html
html
Copiar código
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Banco Digital</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body class="center">
  <div class="welcome-card">
    <h1>Banco Digital</h1>
    <p>Plataforma financeira moderna</p>
    <a href="login.html" class="btn">Entrar</a>
  </div>
</body>
</html>
✅ 2️⃣ login.html
html
Copiar código
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Login</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body class="center">
  <form class="auth-card" id="loginForm">
    <h2>Entrar</h2>
    <input type="email" placeholder="Email" required>
    <input type="password" placeholder="Senha" required>
    <button type="submit">Acessar</button>
    <p id="loginMessage"></p>
  </form>

  <script src="js/auth.js"></script>
</body>
</html>
✅ 3️⃣ dashboard.html
html
Copiar código
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Dashboard</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <aside class="sidebar">
    <h2>Banco</h2>
    <nav>
      <a href="dashboard.html">Dashboard</a>
      <a href="accounts.html">Contas</a>
      <a href="cards.html">Cartões</a>
      <a href="transactions.html">Transações</a>
      <a href="pix.html">Pix</a>
      <a href="loans.html">Empréstimos</a>
      <a href="investments.html">Investimentos</a>
      <a href="support.html">Suporte</a>
      <a href="profile.html">Perfil</a>
    </nav>
  </aside>

  <main class="content">
    <h1>Resumo Financeiro</h1>

    <div class="grid">
      <div class="card">
        <h3>Saldo Total</h3>
        <p id="totalBalance">R$ 0,00</p>
      </div>
      <div class="card">
        <h3>Cartões Ativos</h3>
        <p id="cardsCount">0</p>
      </div>
      <div class="card">
        <h3>Pix do Mês</h3>
        <p id="pixMonth">R$ 0,00</p>
      </div>
      <div class="card">
        <h3>Faturas Pendentes</h3>
        <p id="pendingInvoices">0</p>
      </div>
    </div>
  </main>

  <script src="js/api.js"></script>
  <script src="js/dashboard.js"></script>
</body>
</html>
✅ 4️⃣ accounts.html
html
Copiar código
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Contas</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <aside class="sidebar">
    <h2>Banco</h2>
    <nav>
      <a href="dashboard.html">Dashboard</a>
      <a href="accounts.html" class="active">Contas</a>
      <a href="cards.html">Cartões</a>
      <a href="transactions.html">Transações</a>
      <a href="pix.html">Pix</a>
    </nav>
  </aside>

  <main class="content">
    <h1>Minhas Contas</h1>
    <div id="accountsList" class="list"></div>
  </main>

  <script src="js/api.js"></script>
  <script src="js/accounts.js"></script>
</body>
</html>
✅ 5️⃣ cards.html
html
Copiar código
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Cartões</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <aside class="sidebar">
    <h2>Banco</h2>
    <nav>
      <a href="dashboard.html">Dashboard</a>
      <a href="accounts.html">Contas</a>
      <a href="cards.html" class="active">Cartões</a>
    </nav>
  </aside>

  <main class="content">
    <h1>Meus Cartões</h1>
    <div id="cardsList" class="grid"></div>
  </main>

  <script src="js/api.js"></script>
  <script src="js/cards.js"></script>
</body>
</html>
✅ 6️⃣ pix.html
html
Copiar código
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Pix</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <aside class="sidebar">
    <h2>Banco</h2>
    <nav>
      <a href="dashboard.html">Dashboard</a>
      <a href="pix.html" class="active">Pix</a>
    </nav>
  </aside>

  <main class="content">
    <h1>Área Pix</h1>

    <div class="grid">
      <div class="card">
        <h3>Enviar Pix</h3>
        <input type="text" placeholder="Chave Pix">
        <input type="number" placeholder="Valor">
        <button>Enviar</button>
      </div>

      <div class="card">
        <h3>Minhas Chaves</h3>
        <ul id="pixKeys"></ul>
      </div>
    </div>
  </main>

  <script src="js/api.js"></script>
  <script src="js/pix.js"></script>
</body>
</html>
✅ 7️⃣ transactions.html
html
Copiar código
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Transações</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <aside class="sidebar">
    <h2>Banco</h2>
    <nav>
      <a href="dashboard.html">Dashboard</a>
      <a href="transactions.html" class="active">Transações</a>
    </nav>
  </aside>

  <main class="content">
    <h1>Histórico de Transações</h1>
    <table class="table">
      <thead>
        <tr>
          <th>Data</th>
          <th>Descrição</th>
          <th>Tipo</th>
          <th>Valor</th>
          <th>Status</th>
        </tr>
      </thead>
      <tbody id="transactionsTable"></tbody>
    </table>
  </main>

  <script src="js/api.js"></script>
  <script src="js/transactions.js"></script>
</body>
</html>
✅ 8️⃣ loans.html
html
Copiar código
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Empréstimos</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <aside class="sidebar">
    <h2>Banco</h2>
    <nav>
      <a href="dashboard.html">Dashboard</a>
      <a href="loans.html" class="active">Empréstimos</a>
    </nav>
  </aside>

  <main class="content">
    <h1>Meus Empréstimos</h1>
    <div id="loansList" class="list"></div>
  </main>

  <script src="js/api.js"></script>
  <script src="js/loans.js"></script>
</body>
</html>
✅ 9️⃣ investments.html
html
Copiar código
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Investimentos</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <aside class="sidebar">
    <h2>Banco</h2>
    <nav>
      <a href="dashboard.html">Dashboard</a>
      <a href="investments.html" class="active">Investimentos</a>
    </nav>
  </aside>

  <main class="content">
    <h1>Investimentos</h1>
    <div id="investmentsList" class="grid"></div>
  </main>

  <script src="js/api.js"></script>
  <script src="js/investments.js"></script>
</body>
</html>
✅ 🔟 support.html
html
Copiar código
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Suporte</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <aside class="sidebar">
    <h2>Banco</h2>
    <nav>
      <a href="dashboard.html">Dashboard</a>
      <a href="support.html" class="active">Suporte</a>
    </nav>
  </aside>

  <main class="content">
    <h1>Central de Atendimento</h1>
    <textarea placeholder="Descreva seu problema"></textarea>
    <button>Abrir Chamado</button>
  </main>

  <script src="js/support.js"></script>
</body>
</html>
✅ 1️⃣1️⃣ profile.html
html
Copiar código
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Perfil</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <aside class="sidebar">
    <h2>Banco</h2>
    <nav>
      <a href="dashboard.html">Dashboard</a>
      <a href="profile.html" class="active">Perfil</a>
    </nav>
  </aside>

  <main class="content">
    <h1>Meu Perfil</h1>
    <div class="card">
      <p><strong>Nome:</strong> Usuário Teste</p>
      <p><strong>Email:</strong> teste@email.com</p>
      <button>Sair</button>
    </div>
  </main>
</body>
</html>
🎨 CSS COMPLETO — css/style.css
css
Copiar código
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Inter", Arial, sans-serif;
}

body {
  background: #f4f6fb;
  color: #222;
}

.center {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
}

.welcome-card,
.auth-card {
  background: white;
  padding: 40px;
  border-radius: 16px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
  width: 350px;
  text-align: center;
}

.auth-card input {
  width: 100%;
  padding: 12px;
  margin: 10px 0;
  border-radius: 8px;
  border: 1px solid #ddd;
}

button,
.btn {
  background: #6c2bd9;
  color: white;
  border: none;
  padding: 12px 18px;
  border-radius: 8px;
  cursor: pointer;
  text-decoration: none;
  display: inline-block;
  width: 100%;
  font-weight: 600;
}

button:hover,
.btn:hover {
  background: #5821b5;
}

.sidebar {
  position: fixed;
  left: 0;
  top: 0;
  width: 240px;
  height: 100vh;
  background: #6c2bd9;
  color: white;
  padding: 30px 20px;
}

.sidebar h2 {
  margin-bottom: 30px;
}

.sidebar nav a {
  display: block;
  color: white;
  text-decoration: none;
  padding: 12px 10px;
  border-radius: 8px;
  margin-bottom: 6px;
}

.sidebar nav a:hover,
.sidebar nav a.active {
  background: rgba(255,255,255,0.2);
}

.content {
  margin-left: 260px;
  padding: 30px;
}

h1 {
  margin-bottom: 20px;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 20px;
}

.card {
  background: white;
  padding: 20px;
  border-radius: 16px;
  box-shadow: 0 6px 20px rgba(0,0,0,0.08);
}

.list .item {
  background: white;
  padding: 15px;
  border-radius: 12px;
  margin-bottom: 10px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.06);
}

.table {
  width: 100%;
  background: white;
  border-radius: 12px;
  overflow: hidden;
  border-collapse: collapse;
}

.table th,
.table td {
  padding: 14px;
  border-bottom: 1px solid #eee;
  text-align: left;
}

.table th {
  background: #f0f2f7;
  font-weight: 600;
}
⚙️ JAVASCRIPT — BACKEND MOCK + UI
✅ js/api.js
javascript
Copiar código
const API = {
  getDashboard() {
    return Promise.resolve({
      totalBalance: 12540.75,
      cardsCount: 3,
      pixMonth: 4320.00,
      pendingInvoices: 2
    });
  },

  getAccounts() {
    return Promise.resolve([
      { id: 1, number: "000123", type: "Conta Corrente", balance: 8400.50 },
      { id: 2, number: "000456", type: "Conta Poupança", balance: 4130.25 }
    ]);
  },

  getCards() {
    return Promise.resolve([
      { id: 1, brand: "Visa", last4: "1234", limit: 5000 },
      { id: 2, brand: "Mastercard", last4: "9876", limit: 8000 }
    ]);
  },

  getTransactions() {
    return Promise.resolve([
      { id: 1, date: "2026-01-10", description: "Pix recebido", type: "Crédito", amount: 1200, status: "Concluído" },
      { id: 2, date: "2026-01-09", description: "Compra Mercado", type: "Débito", amount: -350, status: "Concluído" },
      { id: 3, date: "2026-01-08", description: "Netflix", type: "Débito", amount: -39.90, status: "Concluído" }
    ]);
  },

  getPixKeys() {
    return Promise.resolve(["email@email.com", "+55999999999", "cpf"]);
  },

  getLoans() {
    return Promise.resolve([
      { id: 1, type: "Pessoal", amount: 15000, status: "Ativo" },
      { id: 2, type: "Veículo", amount: 42000, status: "Quitado" }
    ]);
  },

  getInvestments() {
    return Promise.resolve([
      { id: 1, product: "CDB Banco X", value: 5400 },
      { id: 2, product: "Tesouro Selic", value: 7800 }
    ]);
  }
};
✅ js/auth.js
javascript
Copiar código
document.getElementById("loginForm").addEventListener("submit", e => {
  e.preventDefault();
  const msg = document.getElementById("loginMessage");
  msg.textContent = "Login realizado com sucesso!";
  msg.style.color = "green";

  setTimeout(() => {
    window.location.href = "dashboard.html";
  }, 1000);
});
✅ js/dashboard.js
javascript
Copiar código
API.getDashboard().then(data => {
  document.getElementById("totalBalance").textContent = "R$ " + data.totalBalance.toFixed(2);
  document.getElementById("cardsCount").textContent = data.cardsCount;
  document.getElementById("pixMonth").textContent = "R$ " + data.pixMonth.toFixed(2);
  document.getElementById("pendingInvoices").textContent = data.pendingInvoices;
});
✅ js/accounts.js
javascript
Copiar código
API.getAccounts().then(accounts => {
  const list = document.getElementById("accountsList");
  accounts.forEach(acc => {
    const div = document.createElement("div");
    div.className = "item";
    div.innerHTML = `
      <strong>${acc.type}</strong><br>
      Conta: ${acc.number}<br>
      Saldo: R$ ${acc.balance.toFixed(2)}
    `;
    list.appendChild(div);
  });
});
✅ js/cards.js
javascript
Copiar código
API.getCards().then(cards => {
  const list = document.getElementById("cardsList");
  cards.forEach(card => {
    const div = document.createElement("div");
    div.className = "card";
    div.innerHTML = `
      <h3>${card.brand}</h3>
      <p>Final: **** ${card.last4}</p>
      <p>Limite: R$ ${card.limit.toFixed(2)}</p>
    `;
    list.appendChild(div);
  });
});
✅ js/pix.js
javascript
Copiar código
API.getPixKeys().then(keys => {
  const ul = document.getElementById("pixKeys");
  keys.forEach(key => {
    const li = document.createElement("li");
    li.textContent = key;
    ul.appendChild(li);
  });
});
✅ js/transactions.js
javascript
Copiar código
API.getTransactions().then(transactions => {
  const tbody = document.getElementById("transactionsTable");
  transactions.forEach(tx => {
    const tr = document.createElement("tr");
    tr.innerHTML = `
      <td>${tx.date}</td>
      <td>${tx.description}</td>
      <td>${tx.type}</td>
      <td>${tx.amount < 0 ? "-" : ""}R$ ${Math.abs(tx.amount).toFixed(2)}</td>
      <td>${tx.status}</td>
    `;
    tbody.appendChild(tr);
  });
});
✅ js/loans.js
javascript
Copiar código
API.getLoans().then(loans => {
  const list = document.getElementById("loansList");
  loans.forEach(loan => {
    const div = document.createElement("div");
    div.className = "item";
    div.innerHTML = `
      <strong>${loan.type}</strong><br>
      Valor: R$ ${loan.amount.toFixed(2)}<br>
      Status: ${loan.status}
    `;
    list.appendChild(div);
  });
});
✅ js/investments.js
javascript
Copiar código
API.getInvestments().then(investments => {
  const list = document.getElementById("investmentsList");
  investments.forEach(inv => {
    const div = document.createElement("div");
    div.className = "card";
    div.innerHTML = `
      <h3>${inv.product}</h3>
      <p>Valor aplicado: R$ ${inv.value.toFixed(2)}</p>
    `;
    list.appendChild(div);
  });
});
✅ js/support.js
javascript
Copiar código
document.querySelector("button").addEventListener("click", () => {
  alert("Chamado aberto com sucesso!");
});
