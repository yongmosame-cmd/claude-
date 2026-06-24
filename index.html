<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>土豆泥的体重小屋</title>
<link rel="apple-touch-icon" href="icon.png">
<link rel="icon" href="icon.png">
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body {
    font-family: 'PingFang SC', 'Hiragino Sans', 'Microsoft YaHei', sans-serif;
    background: #fdf6f0;
    color: #4a3a2e;
    padding: 20px 16px 60px;
  }
  .wrap { max-width: 420px; margin: 0 auto; }
  .header { text-align: center; margin-bottom: 20px; }
  .eyebrow {
    font-size: 11px; color: #c08552; letter-spacing: 4px;
    margin-bottom: 6px; font-weight: 600;
  }
  .cat-face { font-size: 30px; letter-spacing: 1px; }
  .card {
    background: linear-gradient(135deg, #fff9f4, #fef0e4);
    border-radius: 20px; padding: 24px 20px; margin-bottom: 16px;
    border: 1px solid #f5e4d3; box-shadow: 0 8px 24px rgba(192,133,82,0.1);
  }
  .date-label { font-size: 13px; color: #a8825e; margin-bottom: 10px; }
  .input-row { display: flex; gap: 10px; margin-bottom: 12px; }
  input[type="number"], input[type="date"] {
    border: 1.5px solid #f0ddc8; border-radius: 14px; font-size: 16px;
    outline: none; background: #fff; color: #4a3a2e; font-family: inherit;
  }
  input[type="number"] { flex: 1; padding: 14px 16px; }
  input[type="date"] { width: 100%; padding: 8px 10px; font-size: 13px; color: #a8825e; background: #fffdfb; }
  button {
    padding: 14px 22px; border-radius: 14px; border: none;
    background: #d99a5b; color: #fff; font-size: 15px; font-weight: 600;
    cursor: pointer; font-family: inherit;
  }
  .save-status { font-size: 12px; color: #d99a5b; margin-top: 8px; text-align: center; min-height: 16px; }
  .stats-row { display: flex; gap: 10px; margin-bottom: 16px; }
  .stat-box {
    flex: 1; background: #fff; border-radius: 16px; padding: 16px;
    border: 1px solid #f5e4d3; text-align: center; cursor: default;
  }
  .stat-box.goal { cursor: pointer; }
  .stat-value { font-size: 22px; font-weight: 700; color: #4a3a2e; }
  .stat-label { font-size: 11px; color: #a8825e; margin-top: 2px; }
  .down { color: #5ba888; }
  .up { color: #d9785b; }
  .goal-input-row {
    background: #fff; border-radius: 16px; padding: 16px; margin-bottom: 16px;
    border: 1px solid #f5e4d3; display: none; gap: 8px;
  }
  .goal-input-row.show { display: flex; }
  .goal-input-row input { flex: 1; padding: 10px 12px; border-radius: 10px;
    border: 1px solid #f0ddc8; font-size: 14px; outline: none; font-family: inherit; }
  .goal-input-row button { padding: 10px 18px; border-radius: 10px; font-size: 13px; }
  .chart-card, .history-card {
    background: #fff; border-radius: 20px; padding: 20px;
    border: 1px solid #f5e4d3; margin-bottom: 16px;
  }
  .section-label { font-size: 13px; color: #a8825e; margin-bottom: 14px; font-weight: 600; }
  .bars { display: flex; align-items: flex-end; gap: 8px; height: 100px; margin-bottom: 8px; }
  .bar-col { flex: 1; display: flex; flex-direction: column; align-items: center; justify-content: flex-end; height: 100%; }
  .bar-val { font-size: 10px; color: #a8825e; margin-bottom: 4px; }
  .bar {
    width: 100%; max-width: 28px;
    background: linear-gradient(180deg, #f0b884, #d99a5b);
    border-radius: 8px 8px 4px 4px; transition: height 0.4s ease;
  }
  .bar-labels { display: flex; gap: 8px; }
  .bar-labels span { flex: 1; text-align: center; font-size: 10px; color: #c0a890; }
  .empty-state { font-size: 13px; color: #c0a890; text-align: center; padding: 20px 0; }
  .history-item {
    display: flex; justify-content: space-between; align-items: center;
    padding: 10px 12px; background: #fdf6f0; border-radius: 12px; margin-bottom: 8px;
  }
  .history-item:last-child { margin-bottom: 0; }
  .history-date { font-size: 13px; color: #6b5544; }
  .history-right { display: flex; align-items: center; gap: 10px; }
  .history-weight { font-size: 14px; font-weight: 600; color: #4a3a2e; }
  .delete-btn {
    border: none; background: transparent; color: #d99a5b;
    font-size: 12px; cursor: pointer; padding: 4px; font-family: inherit;
  }
</style>
</head>
<body>
  <div class="wrap">
    <div class="header">
      <div class="eyebrow">土豆泥的体重小屋</div>
      <div class="cat-face" id="catFace">(=^-ω-^=)</div>
    </div>

    <div class="card">
      <div class="date-label" id="dateLabel"></div>
      <div class="input-row">
        <input type="number" id="weightInput" inputmode="decimal" step="0.1" placeholder="输入体重 kg">
        <button onclick="handleSave()">记录</button>
      </div>
      <input type="date" id="dateInput">
      <div class="save-status" id="saveStatus"></div>
    </div>

    <div class="stats-row">
      <div class="stat-box">
        <div class="stat-value" id="todayVal">--</div>
        <div class="stat-label">今日 (kg)</div>
      </div>
      <div class="stat-box">
        <div class="stat-value" id="trendVal">--</div>
        <div class="stat-label">较上次</div>
      </div>
      <div class="stat-box goal" onclick="toggleGoalInput()">
        <div class="stat-value" id="goalVal">设置</div>
        <div class="stat-label">目标 (kg)</div>
      </div>
    </div>

    <div class="goal-input-row" id="goalInputRow">
      <input type="number" step="0.1" id="goalInput" placeholder="目标体重 kg">
      <button onclick="handleSetGoal()">保存</button>
    </div>

    <div class="chart-card" id="chartCard" style="display:none">
      <div class="section-label">近期趋势</div>
      <div class="bars" id="bars"></div>
      <div class="bar-labels" id="barLabels"></div>
    </div>

    <div class="history-card">
      <div class="section-label">历史记录</div>
      <div id="historyList"></div>
    </div>
  </div>

<script>
  const STORAGE_KEY = 'weight-log-data';

  function loadData() {
    try {
      const raw = localStorage.getItem(STORAGE_KEY);
      if (raw) return JSON.parse(raw);
    } catch (e) {}
    return { entries: {}, goal: '' };
  }

  function saveData(data) {
    try {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(data));
      showStatus('已保存');
    } catch (e) {
      showStatus('保存失败，再试一次');
    }
  }

  let data = loadData();

  function formatDate(d) {
    const y = d.getFullYear();
    const m = String(d.getMonth() + 1).padStart(2, '0');
    const day = String(d.getDate()).padStart(2, '0');
    return `${y}-${m}-${day}`;
  }

  function formatDisplayDate(dateStr) {
    const d = new Date(dateStr + 'T00:00:00');
    const weekdays = ['周日','周一','周二','周三','周四','周五','周六'];
    return `${d.getMonth()+1}月${d.getDate()}日 ${weekdays[d.getDay()]}`;
  }

  function showStatus(msg) {
    const el = document.getElementById('saveStatus');
    el.textContent = msg;
    setTimeout(() => { el.textContent = ''; }, 1500);
  }

  function getSortedDates() {
    return Object.keys(data.entries).sort((a, b) => a < b ? 1 : -1);
  }

  function render() {
    const today = formatDate(new Date());
    document.getElementById('dateInput').max = today;
    if (!document.getElementById('dateInput').value) {
      document.getElementById('dateInput').value = today;
    }
    const selectedDate = document.getElementById('dateInput').value;
    document.getElementById('dateLabel').textContent = formatDisplayDate(selectedDate);

    const sorted = getSortedDates();
    const todayVal = data.entries[today];
    document.getElementById('todayVal').textContent = todayVal !== undefined ? todayVal : '--';

    let trend = null;
    if (sorted.length >= 2) {
      trend = (data.entries[sorted[0]] - data.entries[sorted[1]]).toFixed(1);
    }
    const trendEl = document.getElementById('trendVal');
    if (trend !== null) {
      const t = parseFloat(trend);
      trendEl.textContent = t > 0 ? `+${trend}` : trend;
      trendEl.className = 'stat-value ' + (t < 0 ? 'down' : t > 0 ? 'up' : '');
    } else {
      trendEl.textContent = '--';
      trendEl.className = 'stat-value';
    }

    document.getElementById('goalVal').textContent = data.goal || '设置';

    // cat mood
    let mood = '(=^-ω-^=)';
    if (todayVal !== undefined) {
      if (trend !== null && parseFloat(trend) < 0) mood = '(=^･ω･^=)';
      else if (trend !== null && parseFloat(trend) === 0) mood = '(=^‐ω‐^=)';
      else mood = '(=￣ω￣=)';
    }
    document.getElementById('catFace').textContent = mood;

    // chart
    const last7 = sorted.slice(0, 7).reverse();
    const chartCard = document.getElementById('chartCard');
    if (last7.length > 0) {
      chartCard.style.display = 'block';
      const vals = last7.map(d => data.entries[d]);
      const max = Math.max(...vals) + 1;
      const min = Math.min(...vals) - 1;
      const range = (max - min) || 1;
      const barsEl = document.getElementById('bars');
      const labelsEl = document.getElementById('barLabels');
      barsEl.innerHTML = '';
      labelsEl.innerHTML = '';
      last7.forEach(date => {
        const val = data.entries[date];
        const heightPct = ((val - min) / range) * 80 + 15;
        const col = document.createElement('div');
        col.className = 'bar-col';
        col.innerHTML = `<div class="bar-val">${val}</div><div class="bar" style="height:${heightPct}%"></div>`;
        barsEl.appendChild(col);
        const lbl = document.createElement('span');
        lbl.textContent = date.slice(5).replace('-', '/');
        labelsEl.appendChild(lbl);
      });
    } else {
      chartCard.style.display = 'none';
    }

    // history
    const historyList = document.getElementById('historyList');
    if (sorted.length === 0) {
      historyList.innerHTML = '<div class="empty-state">还没有记录，今天开始第一条吧</div>';
    } else {
      historyList.innerHTML = sorted.slice(0, 14).map(date => `
        <div class="history-item">
          <span class="history-date">${formatDisplayDate(date)}</span>
          <div class="history-right">
            <span class="history-weight">${data.entries[date]} kg</span>
            <button class="delete-btn" onclick="handleDelete('${date}')">删除</button>
          </div>
        </div>
      `).join('');
    }
  }

  function handleSave() {
    const input = document.getElementById('weightInput');
    const val = parseFloat(input.value);
    if (!val || val <= 0 || val > 500) {
      showStatus('请输入有效体重');
      return;
    }
    const date = document.getElementById('dateInput').value;
    data.entries[date] = val;
    saveData(data);
    input.value = '';
    render();
  }

  function handleDelete(date) {
    delete data.entries[date];
    saveData(data);
    render();
  }

  function toggleGoalInput() {
    const row = document.getElementById('goalInputRow');
    row.classList.toggle('show');
    document.getElementById('goalInput').value = data.goal || '';
  }

  function handleSetGoal() {
    data.goal = document.getElementById('goalInput').value;
    saveData(data);
    document.getElementById('goalInputRow').classList.remove('show');
    render();
  }

  document.getElementById('weightInput').addEventListener('keydown', e => {
    if (e.key === 'Enter') handleSave();
  });
  document.getElementById('dateInput').addEventListener('change', render);

  render();
</script>
</body>
</html>
