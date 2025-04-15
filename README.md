<!DOCTYPE html>
<html lang="kk">
<head>
  <meta charset="UTF-8">
  <title>Алисламның сайты</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #fff;
      color: #a30000;
      margin: 0;
      padding: 0;
    }

    nav {
      background: #a30000;
      padding: 10px;
      text-align: center;
      display: none;
    }

    nav button {
      color: white;
      background: none;
      border: none;
      margin: 0 15px;
      font-size: 16px;
      cursor: pointer;
    }

    .section {
      display: none;
      padding: 30px;
    }

    .active {
      display: block;
    }

    .profile-pic {
      width: 200px;
      border-radius: 10px;
      margin-top: 20px;
    }

    .login-page {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #fff0f0;
    }

    .login-container {
      text-align: center;
      border: 2px solid #a30000;
      padding: 30px;
      border-radius: 10px;
    }

    input, button {
      padding: 8px;
      margin-top: 10px;
    }

    .reviews p {
      background: #ffecec;
      padding: 10px;
      border-left: 4px solid #a30000;
      margin: 10px 0;
    }
  </style>
</head>
<body>

  <!-- Кіру парағы -->
  <div class="login-page" id="login-page">
    <div class="login-container">
      <h1>Қош келдіңіз!</h1>
      <p>Кіру үшін құпиясөзді енгізіңіз:</p>
      <input type="password" id="password" placeholder="Құпиясөз">
      <br>
      <button onclick="checkPassword()">Кіру</button>
      <p id="error"></p>
    </div>
  </div>

  <!-- Навигация -->
  <nav id="nav">
    <button onclick="showSection('home')">Басты бет</button>
    <button onclick="showSection('features')">Өзім жайлы</button>
    <button onclick="showSection('reviews')">Пікірлер</button>
  </nav>

  <!-- Басты бет -->
  <div id="home" class="section">
    <h1>Сәлем, менің атым Алислам!</h1>
    <p>Мен 18 жастамын, Нархоз университетінің 1 курс студентімін.</p>
    <img src="6bc06484-ebd4-408e-ba85-5a8ecf83c42c.jpg" alt="Алислам" class="profile-pic">
  </div>

  <!-- Өзім жайлы -->
  <div id="features" class="section">
    <h1>Өзім жайлы</h1>
    <p><strong>Хобби:</strong> футбол, волейбол, FIFA 🎮⚽🏐</p>
    <p><strong>Оқу:</strong> Нархоз университетінде "Статистика және Data Science" мамандығында оқимын.</p>
    <p><strong>ҰБТ:</strong> 111 балл жинадым</p>

    <h2>Нархоз туралы</h2>
    <p>Нархоз университеті — Қазақстандағы экономика, бизнес, құқық және технология салаларындағы үздік жоғары оқу орындарының бірі. Университет Алматы қаласында орналасқан және 1963 жылдан бері білім беріп келеді.</p>
    <p>Университет заманауи инфрақұрылыммен жабдықталған: жаңа зертханалар, үлкен кітапхана, IT-хаб, коворкингтер және демалыс аймақтары бар. Сонымен қатар, студенттерге арналған түрлі клубтар мен жобалар жұмыс істейді.</p>
    <p>Оқу процесі ағылшын, қазақ және орыс тілдерінде өтеді. Нархоз халықаралық стандарттарға сәйкес білім беріп, шетелдік университеттермен тығыз байланыс орнатқан. Студенттер алмасу бағдарламалары арқылы шетелде оқи алады.</p>
    <p>Мұнда оқыту тек теориямен шектелмейді – нақты жобалармен жұмыс, кәсіпорындармен серіктестік, тәжірибеден өту мүмкіндіктері де қарастырылған. Бұл студенттерді болашақ мамандықтарына нақты дайындайды.</p>

    <h2>"Статистика және Data Science" бағыты туралы</h2>
    <p>Бұл мамандық — қазіргі заманның ең өзекті бағыттарының бірі. Біз мәліметтерді жинау, өңдеу, талдау және сол арқылы шешім қабылдауды үйренеміз. Data Science — жасанды интеллект, машиналық оқыту, үлкен мәліметтер (big data) және аналитикамен тығыз байланысты.</p>
    <p>Оқу барысында Python, R, SQL секілді программалау тілдерін меңгереміз. Сонымен қатар, Excel, Tableau, Power BI секілді аналитикалық құралдармен жұмыс істейміз.</p>
    <p>Бізге ықтималдық теориясы, математикалық статистика, деректер құрылымы, машиналық оқыту, нейрондық желілер, бизнес-аналитика және визуализация сияқты пәндер өтеді.</p>
    <p>Бұл салада мамандарға сұраныс өте жоғары. Болашақта деректер ғалымы, аналитик, machine learning инженер, BI маманы сияқты беделді және табысты қызметтер атқара аламын.</p>
    <p>Ең бастысы — бұл бағыт маған өте қызықты. Әр күн сайын жаңа бір нәрсе үйреніп, нақты деректермен жұмыс істеу маған мотивация береді!</p>
  </div>

  <!-- Пікірлер -->
  <div id="reviews" class="section">
    <h1>Пікірлер</h1>
    <div class="reviews">
      <p>🔥 "Керемет сайт, Алислам мықтысың!" — Досы</p>
      <p>💬 "Қарапайым, бірақ ерекше. Ұнайды!" — Топтастары</p>
    </div>
    <form onsubmit="event.preventDefault(); addReview();">
      <input type="text" id="reviewInput" placeholder="Пікір қалдырыңыз">
      <button>Жіберу</button>
    </form>
  </div>

  <script>
    function checkPassword() {
      const password = document.getElementById('password').value;
      const error = document.getElementById('error');
      if (password === 'Dolgono') {
        document.getElementById('login-page').style.display = 'none';
        document.getElementById('nav').style.display = 'block';
        showSection('home');
      } else {
        error.textContent = 'Құпиясөз қате!';
        error.style.color = 'red';
      }
    }

    function showSection(id) {
      const sections = document.querySelectorAll('.section');
      sections.forEach(s => s.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }

    function addReview() {
      const input = document.getElementById('reviewInput');
      const text = input.value.trim();
      if (text !== '') {
        const div = document.querySelector('.reviews');
        const p = document.createElement('p');
        p.textContent = `📝 "${text}" — Қонақ`;
        div.appendChild(p);
        input.value = '';
      }
    }
  </script>

</body>
</html>
