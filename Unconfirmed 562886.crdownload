/* ===========================================================
   Bahi — Shopkeeper Ledger (Vanilla JS SPA)
   =========================================================== */

/* ---------- Icons ---------- */
const I = {
  home: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 10.5L12 3l9 7.5"/><path d="M5 9.5V21h14V9.5"/></svg>',
  ledger: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h13a3 3 0 0 1 3 3v13H7a3 3 0 0 1-3-3V4z"/><path d="M8 8h8M8 12h8M8 16h5"/></svg>',
  bill: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M6 2h12v20l-3-2-3 2-3-2-3 2V2z"/><path d="M9 7h6M9 11h6M9 15h4"/></svg>',
  chart: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 3v18h18"/><path d="M7 14l4-4 3 3 5-6"/></svg>',
  tools: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="3"/><path d="M19.4 15a1.7 1.7 0 0 0 .3 1.8l.1.1a2 2 0 1 1-2.8 2.8l-.1-.1a1.7 1.7 0 0 0-1.8-.3 1.7 1.7 0 0 0-1 1.5V21a2 2 0 1 1-4 0v-.1a1.7 1.7 0 0 0-1.1-1.5 1.7 1.7 0 0 0-1.8.3l-.1.1a2 2 0 1 1-2.8-2.8l.1-.1a1.7 1.7 0 0 0 .3-1.8 1.7 1.7 0 0 0-1.5-1H3a2 2 0 1 1 0-4h.1a1.7 1.7 0 0 0 1.5-1.1 1.7 1.7 0 0 0-.3-1.8l-.1-.1a2 2 0 1 1 2.8-2.8l.1.1a1.7 1.7 0 0 0 1.8.3H9a1.7 1.7 0 0 0 1-1.5V3a2 2 0 1 1 4 0v.1a1.7 1.7 0 0 0 1 1.5 1.7 1.7 0 0 0 1.8-.3l.1-.1a2 2 0 1 1 2.8 2.8l-.1.1a1.7 1.7 0 0 0-.3 1.8V9a1.7 1.7 0 0 0 1.5 1H21a2 2 0 1 1 0 4h-.1a1.7 1.7 0 0 0-1.5 1z"/></svg>',
  plus: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M12 5v14M5 12h14"/></svg>',
  search: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="11" cy="11" r="7"/><path d="M21 21l-4.3-4.3"/></svg>',
  sun: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="4"/><path d="M12 2v2M12 20v2M4.93 4.93l1.41 1.41M17.66 17.66l1.41 1.41M2 12h2M20 12h2M4.93 19.07l1.41-1.41M17.66 6.34l1.41-1.41"/></svg>',
  moon: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 12.8A9 9 0 1 1 11.2 3a7 7 0 0 0 9.8 9.8z"/></svg>',
  logout: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 21H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h4"/><path d="M16 17l5-5-5-5M21 12H9"/></svg>',
  trash: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 6h18M8 6V4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v2M19 6l-1 14a2 2 0 0 1-2 2H8a2 2 0 0 1-2-2L5 6"/></svg>',
  check: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12l5 5L20 7"/></svg>',
  x: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M18 6L6 18M6 6l12 12"/></svg>',
  info: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><path d="M12 8v.01M11 12h1v4"/></svg>',
  whatsapp: '<svg viewBox="0 0 24 24" fill="currentColor"><path d="M17.5 14.4c-.3-.1-1.7-.8-2-.9-.3-.1-.5-.1-.7.2-.2.3-.7.9-.9 1.1-.2.2-.3.2-.6.1-.3-.1-1.2-.4-2.3-1.4-.8-.7-1.4-1.6-1.6-1.9-.2-.3 0-.4.1-.6l.4-.5c.1-.2.2-.3.3-.5.1-.2 0-.4 0-.5l-.7-1.7c-.2-.4-.4-.4-.5-.4h-.5c-.2 0-.5.1-.7.3-.3.3-1 1-1 2.4s1 2.8 1.2 3c.1.2 2 3 4.8 4.2.7.3 1.2.5 1.6.6.7.2 1.3.2 1.8.1.5-.1 1.7-.7 1.9-1.3.2-.7.2-1.2.2-1.3-.1-.1-.3-.2-.6-.3M12 2C6.5 2 2 6.5 2 12c0 1.7.5 3.4 1.3 4.8L2 22l5.3-1.4c1.4.7 3 1.1 4.7 1.1 5.5 0 10-4.5 10-10S17.5 2 12 2"/></svg>',
  edit: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M11 4H5a2 2 0 0 0-2 2v13a2 2 0 0 0 2 2h13a2 2 0 0 0 2-2v-6"/><path d="M18.4 2.6a2 2 0 0 1 2.8 2.8L12 14.6l-4 1 1-4 9.4-9z"/></svg>',
  download: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><path d="M7 10l5 5 5-5M12 15V3"/></svg>',
  upload: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><path d="M17 8l-5-5-5 5M12 3v12"/></svg>',
  calc: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="4" y="2" width="16" height="20" rx="2"/><path d="M8 6h8M8 10h.01M12 10h.01M16 10h.01M8 14h.01M12 14h.01M16 14h.01M8 18h.01M12 18h.01M16 18h.01"/></svg>',
  rupee: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M6 4h12M6 8h12M9 4c2.5 0 4 1.5 4 4s-1.5 4-4 4H6l8 8"/></svg>',
  empty: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 7l9-4 9 4M3 7v10l9 4 9-4V7M3 7l9 4 9-4M12 11v10"/></svg>',
};

/* ---------- Storage ---------- */
const DB = {
  USERS: 'bahi_users',
  SESSION: 'bahi_session',
  THEME: 'bahi_theme',
  data: (uid) => `bahi_data_${uid}`,
};
const get = (k, fb) => { try { return JSON.parse(localStorage.getItem(k)) ?? fb; } catch { return fb; } };
const set = (k, v) => localStorage.setItem(k, JSON.stringify(v));

/* ---------- State ---------- */
let state = {
  user: null,
  page: 'dashboard',
  entries: [], // {id,name,phone,items:[{name,qty,price}],total,status,date,paidAt}
  filter: 'all',
  search: '',
  reportRange: 'week',
};

const fmt = (n) => '₹' + (Number(n) || 0).toLocaleString('en-IN', { maximumFractionDigits: 0 });
const initials = (s) => (s||'?').trim().split(/\s+/).map(w=>w[0]).slice(0,2).join('').toUpperCase();
const uid = () => Date.now().toString(36) + Math.random().toString(36).slice(2,7);
const todayKey = (d=new Date()) => d.toISOString().slice(0,10);

/* ---------- Theme ---------- */
function applyTheme(t) {
  document.documentElement.dataset.theme = t;
  document.querySelector('meta[name=theme-color]').setAttribute('content', t === 'dark' ? '#0b0d12' : '#ffffff');
  set(DB.THEME, t);
}
function toggleTheme() {
  const cur = document.documentElement.dataset.theme;
  applyTheme(cur === 'dark' ? 'light' : 'dark');
  render();
}

/* ---------- Toast ---------- */
function toast(msg, type='success') {
  const c = document.getElementById('toast-container');
  const t = document.createElement('div');
  t.className = 'toast ' + type;
  const ic = type === 'success' ? I.check : type === 'error' ? I.x : I.info;
  t.innerHTML = `<div class="toast-icon">${ic}</div><div>${msg}</div>`;
  c.appendChild(t);
  setTimeout(() => { t.classList.add('hide'); setTimeout(()=>t.remove(), 300); }, 2400);
}

/* ---------- Modal ---------- */
function openModal(html, { center = false } = {}) {
  const root = document.getElementById('modal-root');
  root.innerHTML = `<div class="modal-backdrop"><div class="modal ${center?'center':''}">${center?'':'<div class="modal-handle"></div>'}${html}</div></div>`;
  const bd = root.querySelector('.modal-backdrop');
  bd.addEventListener('click', (e) => { if (e.target === bd) closeModal(); });
  return root.querySelector('.modal');
}
function closeModal() { document.getElementById('modal-root').innerHTML = ''; }

function confirmDialog(title, message, onYes) {
  const m = openModal(`
    <h3 class="modal-title">${title}</h3>
    <p class="text-mute mb-12">${message}</p>
    <div class="row">
      <button class="btn btn-ghost btn-block" data-cancel>Cancel</button>
      <button class="btn btn-primary btn-block" data-ok>Confirm</button>
    </div>
  `, { center: true });
  m.querySelector('[data-cancel]').onclick = closeModal;
  m.querySelector('[data-ok]').onclick = () => { closeModal(); onYes(); };
}

/* ---------- Ripple ---------- */
document.addEventListener('click', (e) => {
  const btn = e.target.closest('.btn-primary');
  if (!btn) return;
  const r = btn.getBoundingClientRect();
  const ripple = document.createElement('span');
  ripple.className = 'ripple';
  const size = Math.max(r.width, r.height);
  ripple.style.width = ripple.style.height = size + 'px';
  ripple.style.left = (e.clientX - r.left - size/2) + 'px';
  ripple.style.top = (e.clientY - r.top - size/2) + 'px';
  btn.appendChild(ripple);
  setTimeout(() => ripple.remove(), 600);
});

/* ---------- Auth ---------- */
function loadSession() {
  const sid = get(DB.SESSION, null);
  if (!sid) return null;
  const users = get(DB.USERS, []);
  return users.find(u => u.id === sid) || null;
}
function saveData() { set(DB.data(state.user.id), state.entries); }
function loadData() { state.entries = get(DB.data(state.user.id), []); }

function login(email, password) {
  const users = get(DB.USERS, []);
  const u = users.find(x => x.email === email.toLowerCase().trim() && x.password === password);
  if (!u) return { ok:false, msg:'Invalid email or password' };
  set(DB.SESSION, u.id);
  state.user = u; loadData();
  return { ok:true };
}
function register(name, email, password) {
  email = email.toLowerCase().trim();
  const users = get(DB.USERS, []);
  if (users.some(u => u.email === email)) return { ok:false, msg:'Email already registered' };
  const u = { id: uid(), name: name.trim(), email, password, createdAt: Date.now() };
  users.push(u); set(DB.USERS, users);
  set(DB.SESSION, u.id);
  state.user = u; state.entries = []; saveData();
  return { ok:true };
}
function logout() {
  localStorage.removeItem(DB.SESSION);
  state.user = null; state.entries = [];
  render();
}

/* ---------- Render Auth ---------- */
function renderAuth() {
  const root = document.getElementById('app');
  root.innerHTML = `
    <div class="auth-wrap">
      <div class="auth-brand">
        <div class="auth-logo">${I.ledger}</div>
        <h1 class="auth-title">Bahi</h1>
        <p class="auth-subtitle">Smart ledger for modern shopkeepers</p>
      </div>
      <div class="auth-card">
        <div class="auth-tabs" data-tab="login">
          <div class="auth-tab-indicator"></div>
          <button class="auth-tab active" data-t="login">Login</button>
          <button class="auth-tab" data-t="register">Register</button>
        </div>
        <form id="auth-form" autocomplete="off">
          <div class="field" data-only="register" style="display:none">
            <label>Full Name</label>
            <input class="input" name="name" placeholder="Your name" />
            <div class="field-error" data-err="name"></div>
          </div>
          <div class="field">
            <label>Email</label>
            <input class="input" name="email" type="email" placeholder="you@shop.com" />
            <div class="field-error" data-err="email"></div>
          </div>
          <div class="field">
            <label>Password</label>
            <input class="input" name="password" type="password" placeholder="••••••••" />
            <div class="field-error" data-err="password"></div>
          </div>
          <button type="submit" class="btn btn-primary btn-block mt-12" id="auth-submit">Login</button>
        </form>
      </div>
      <p class="text-mute text-center mt-16" style="font-size:12.5px">Your data stays on your device, secure & private.</p>
    </div>
  `;

  const form = root.querySelector('#auth-form');
  const submit = root.querySelector('#auth-submit');
  const tabs = root.querySelector('.auth-tabs');
  let mode = 'login';

  tabs.querySelectorAll('.auth-tab').forEach(b => {
    b.onclick = () => {
      mode = b.dataset.t;
      tabs.dataset.tab = mode;
      tabs.querySelectorAll('.auth-tab').forEach(x => x.classList.toggle('active', x === b));
      root.querySelector('[data-only="register"]').style.display = mode === 'register' ? '' : 'none';
      submit.textContent = mode === 'login' ? 'Login' : 'Create Account';
      form.querySelectorAll('.field-error').forEach(e => e.textContent = '');
      form.querySelectorAll('.input').forEach(i => i.classList.remove('error'));
    };
  });

  form.onsubmit = (e) => {
    e.preventDefault();
    const fd = new FormData(form);
    const name = (fd.get('name')||'').toString().trim();
    const email = (fd.get('email')||'').toString().trim();
    const password = (fd.get('password')||'').toString();
    let ok = true;
    const setErr = (k, m) => {
      const i = form.querySelector(`[name=${k}]`);
      const e = form.querySelector(`[data-err=${k}]`);
      if (m) { i.classList.add('error'); e.textContent = m; ok = false; }
      else { i.classList.remove('error'); e.textContent = ''; }
    };
    if (mode === 'register') setErr('name', name.length < 2 ? 'Enter your name' : '');
    setErr('email', /^\S+@\S+\.\S+$/.test(email) ? '' : 'Enter a valid email');
    setErr('password', password.length < 4 ? 'At least 4 characters' : '');
    if (!ok) return;

    const res = mode === 'login' ? login(email, password) : register(name, email, password);
    if (!res.ok) { toast(res.msg, 'error'); return; }
    toast(mode === 'login' ? `Welcome back, ${state.user.name}!` : `Welcome, ${state.user.name}!`);
    render();
  };
}

/* ---------- Render Shell ---------- */
function renderShell() {
  const root = document.getElementById('app');
  const titles = { dashboard:'Dashboard', ledger:'Udhar Book', bill:'New Bill', reports:'Reports', tools:'Tools' };
  const isDark = document.documentElement.dataset.theme === 'dark';
  root.innerHTML = `
    <header class="header">
      <div>
        <div class="header-title">${titles[state.page] || 'Bahi'}</div>
        <div style="font-size:11px;color:var(--text-mute);font-weight:500;margin-top:1px">${state.user.name}</div>
      </div>
      <div class="header-actions">
        <button class="icon-btn" id="theme-toggle" aria-label="Toggle theme">${isDark ? I.sun : I.moon}</button>
        <button class="icon-btn" id="logout-btn" aria-label="Logout">${I.logout}</button>
      </div>
    </header>
    <main id="page-host"></main>
    ${state.page === 'dashboard' || state.page === 'ledger' ? `<button class="fab" id="fab" aria-label="New entry">${I.plus}</button>` : ''}
    <nav class="bottom-nav"><div class="bottom-nav-inner">
      ${navItem('dashboard','Home', I.home)}
      ${navItem('ledger','Udhar', I.ledger)}
      ${navItem('bill','Bill', I.bill)}
      ${navItem('reports','Reports', I.chart)}
      ${navItem('tools','Tools', I.tools)}
    </div></nav>
  `;
  root.querySelector('#theme-toggle').onclick = toggleTheme;
  root.querySelector('#logout-btn').onclick = () => confirmDialog('Logout?', 'You can sign in again anytime.', logout);
  root.querySelectorAll('.nav-item').forEach(b => b.onclick = () => navigate(b.dataset.p));
  const fab = root.querySelector('#fab');
  if (fab) fab.onclick = openEntryModal;
  renderPage();
}
function navItem(p, label, icon) {
  return `<button class="nav-item ${state.page===p?'active':''}" data-p="${p}">${icon}<span>${label}</span></button>`;
}

function navigate(p) {
  if (p === state.page) return;
  const host = document.getElementById('page-host');
  if (host) {
    host.classList.add('page-out');
    setTimeout(() => { state.page = p; renderShell(); }, 160);
  } else {
    state.page = p; renderShell();
  }
}

function renderPage() {
  const host = document.getElementById('page-host');
  if (state.page === 'dashboard') host.innerHTML = pageDashboard();
  else if (state.page === 'ledger') host.innerHTML = pageLedger();
  else if (state.page === 'bill') host.innerHTML = pageBill();
  else if (state.page === 'reports') host.innerHTML = pageReports();
  else if (state.page === 'tools') host.innerHTML = pageTools();

  bindPage();
  // Animate counters
  host.querySelectorAll('[data-count]').forEach(el => animateCount(el));
  // Animate bars
  setTimeout(() => host.querySelectorAll('.bar-fill').forEach(b => b.style.height = b.dataset.h + '%'), 50);
}

/* ---------- Stats ---------- */
function computeStats() {
  let earnings = 0, udhar = 0, todaySales = 0;
  const tk = todayKey();
  state.entries.forEach(e => {
    if (e.status === 'paid') earnings += e.total;
    else udhar += e.total;
    if (e.date.slice(0,10) === tk) todaySales += e.total;
  });
  return { earnings, udhar, todaySales };
}

function animateCount(el) {
  const target = +el.dataset.count;
  const prefix = el.dataset.prefix || '';
  const dur = 700;
  const start = performance.now();
  const tick = (t) => {
    const p = Math.min(1, (t - start) / dur);
    const eased = 1 - Math.pow(1 - p, 3);
    const v = Math.round(target * eased);
    el.textContent = prefix + v.toLocaleString('en-IN');
    if (p < 1) requestAnimationFrame(tick);
  };
  requestAnimationFrame(tick);
}

/* ---------- Pages ---------- */
function pageDashboard() {
  const { earnings, udhar, todaySales } = computeStats();
  const recent = [...state.entries].sort((a,b) => b.date.localeCompare(a.date)).slice(0,5);
  return `
    <div class="page">
      <div class="stats-grid">
        <div class="stat-card featured">
          <div class="stat-icon">${I.rupee}</div>
          <div class="stat-label">Total Earnings</div>
          <div class="stat-value" data-count="${earnings}" data-prefix="₹">₹0</div>
        </div>
        <div class="stat-card">
          <div class="stat-icon">${I.ledger}</div>
          <div class="stat-label">Pending Udhar</div>
          <div class="stat-value" data-count="${udhar}" data-prefix="₹">₹0</div>
        </div>
        <div class="stat-card">
          <div class="stat-icon">${I.chart}</div>
          <div class="stat-label">Today's Sales</div>
          <div class="stat-value" data-count="${todaySales}" data-prefix="₹">₹0</div>
        </div>
      </div>

      <div class="section-title">Quick Actions</div>
      <div class="action-grid">
        <button class="action-tile" data-action="new-udhar"><div class="ic">${I.plus}</div><div><div class="t">New Udhar</div><div class="d">Add a credit entry</div></div></button>
        <button class="action-tile" data-action="new-bill"><div class="ic">${I.bill}</div><div><div class="t">Create Bill</div><div class="d">Generate quick bill</div></div></button>
      </div>

      <div class="section-title">Recent Activity</div>
      ${recent.length ? `<div class="list">${recent.map(entryCard).join('')}</div>` : emptyState('No activity yet', 'Add your first udhar or bill to get started.')}
    </div>
  `;
}

function pageLedger() {
  const filtered = state.entries.filter(e => {
    if (state.filter !== 'all' && e.status !== state.filter) return false;
    if (state.search) {
      const q = state.search.toLowerCase();
      if (!e.name.toLowerCase().includes(q) && !(e.phone||'').includes(q)) return false;
    }
    return true;
  }).sort((a,b) => b.date.localeCompare(a.date));

  return `
    <div class="page">
      <div class="search-wrap">
        <span class="search-icon">${I.search}</span>
        <input class="search-input" id="search-inp" placeholder="Search by name or phone" value="${escapeHtml(state.search)}" />
      </div>
      <div class="chips">
        ${chip('all','All')} ${chip('pending','Pending')} ${chip('paid','Paid')}
      </div>
      ${filtered.length ? `<div class="list">${filtered.map(entryCard).join('')}</div>` : emptyState('No entries found', state.search?'Try a different search term.':'Tap the + button to add your first entry.')}
    </div>
  `;
}
function chip(v, label) {
  return `<button class="chip ${state.filter===v?'active':''}" data-filter="${v}">${label}</button>`;
}

function entryCard(e) {
  const cls = e.status === 'paid' ? 'positive' : 'pending';
  const badge = e.status === 'paid'
    ? `<span class="badge badge-paid"><span class="badge-dot"></span>Paid</span>`
    : `<span class="badge badge-pending"><span class="badge-dot"></span>Pending</span>`;
  const date = new Date(e.date).toLocaleDateString('en-IN', { day:'2-digit', month:'short' });
  return `
    <div class="entry-card" data-id="${e.id}">
      <div class="entry-avatar">${initials(e.name)}</div>
      <div class="entry-body">
        <div class="entry-name">${escapeHtml(e.name)}</div>
        <div class="entry-meta">${badge} · ${date} · ${e.items.length} item${e.items.length>1?'s':''}</div>
      </div>
      <div class="entry-amount ${cls}">${fmt(e.total)}</div>
    </div>
  `;
}

function pageBill() {
  return `
    <div class="page">
      <div class="card">
        <div class="row mb-12">
          <div style="flex:1">
            <label class="text-mute" style="font-size:12px;font-weight:600">Customer Name</label>
            <input class="input mt-12" id="bill-name" placeholder="e.g. Ramesh Kumar" />
          </div>
        </div>
        <div class="field">
          <label class="text-mute" style="font-size:12px;font-weight:600">Phone (optional)</label>
          <input class="input mt-12" id="bill-phone" placeholder="10-digit number" inputmode="numeric" maxlength="10" />
        </div>

        <div class="section-title" style="margin:14px 0 8px">Items</div>
        <div id="bill-items"></div>
        <button class="btn btn-ghost btn-sm" id="add-item">${I.plus}<span>Add Item</span></button>

        <div class="bill-summary">
          <div>
            <div class="text-mute" style="font-size:12px">Total Amount</div>
            <div class="bill-total" id="bill-total">₹0</div>
          </div>
          <div class="row" style="gap:6px">
            <button class="btn btn-ghost btn-sm" id="bill-whatsapp" title="Share on WhatsApp" style="color:#25d366">${I.whatsapp}</button>
          </div>
        </div>

        <div class="row mt-16">
          <button class="btn btn-ghost btn-block" id="bill-paid-save">Save as Paid</button>
          <button class="btn btn-primary btn-block" id="bill-udhar-save">Save as Udhar</button>
        </div>
      </div>
    </div>
  `;
}

function pageReports() {
  const range = state.reportRange;
  const days = range === 'day' ? 1 : range === 'week' ? 7 : 30;
  const buckets = [];
  for (let i = days - 1; i >= 0; i--) {
    const d = new Date(); d.setDate(d.getDate() - i);
    const k = todayKey(d);
    const sum = state.entries.filter(e => e.date.slice(0,10) === k).reduce((a,b) => a + b.total, 0);
    buckets.push({ k, label: d.toLocaleDateString('en-IN',{ day:'2-digit', month:'short'}), sum });
  }
  const max = Math.max(1, ...buckets.map(b => b.sum));
  const total = buckets.reduce((a,b)=>a+b.sum,0);
  const paid = state.entries.filter(e => e.status==='paid').length;
  const pending = state.entries.filter(e => e.status==='pending').length;
  const showLabels = days <= 7;

  return `
    <div class="page">
      <div class="chips">
        ${rchip('day','Today')} ${rchip('week','7 Days')} ${rchip('month','30 Days')}
      </div>
      <div class="card">
        <div class="row" style="justify-content:space-between">
          <div>
            <div class="text-mute" style="font-size:12px">Total in period</div>
            <div style="font-size:24px;font-weight:800;letter-spacing:-0.02em">${fmt(total)}</div>
          </div>
          <div style="text-align:right">
            <div class="text-mute" style="font-size:12px">Entries</div>
            <div style="font-weight:700">${paid} paid · ${pending} pending</div>
          </div>
        </div>
        <div class="chart mt-16">
          ${buckets.map(b => `
            <div class="bar" title="${b.label}: ${fmt(b.sum)}">
              <div class="bar-fill" data-h="${(b.sum/max)*92}" style="height:0%"></div>
              ${showLabels ? `<div class="bar-label">${b.label.split(' ')[0]}</div>` : ''}
            </div>
          `).join('')}
        </div>
      </div>

      <div class="section-title">Export</div>
      <div class="action-grid">
        <button class="action-tile" data-action="export-json"><div class="ic">${I.download}</div><div><div class="t">Export JSON</div><div class="d">Backup full data</div></div></button>
        <button class="action-tile" data-action="export-csv"><div class="ic">${I.download}</div><div><div class="t">Export CSV</div><div class="d">For spreadsheets</div></div></button>
      </div>
    </div>
  `;
}
function rchip(v, label) {
  return `<button class="chip ${state.reportRange===v?'active':''}" data-range="${v}">${label}</button>`;
}

function pageTools() {
  return `
    <div class="page">
      <div class="card">
        <div class="row" style="gap:10px"><div class="ic" style="width:38px;height:38px;border-radius:12px;display:grid;place-items:center;background:var(--primary-soft);color:var(--primary)">${I.calc}</div>
          <div><div style="font-weight:700">Loan Calculator</div><div class="text-mute" style="font-size:12px">Simple interest helper</div></div>
        </div>
        <div class="field mt-16"><label>Principal (₹)</label><input class="input" id="li-p" type="number" inputmode="numeric" placeholder="10000" /></div>
        <div class="row">
          <div class="field" style="flex:1"><label>Rate (% / yr)</label><input class="input" id="li-r" type="number" step="0.1" placeholder="12" /></div>
          <div class="field" style="flex:1"><label>Time (years)</label><input class="input" id="li-t" type="number" step="0.1" placeholder="2" /></div>
        </div>
        <button class="btn btn-primary btn-block" id="li-calc">Calculate</button>
        <div id="li-result"></div>
      </div>

      <div class="section-title">Backup & Restore</div>
      <div class="action-grid">
        <button class="action-tile" data-action="export-json"><div class="ic">${I.download}</div><div><div class="t">Export Data</div><div class="d">Download backup</div></div></button>
        <button class="action-tile" data-action="import-json"><div class="ic">${I.upload}</div><div><div class="t">Import Data</div><div class="d">Restore from JSON</div></div></button>
      </div>

      <div class="section-title">Danger Zone</div>
      <div class="card">
        <div class="row" style="justify-content:space-between">
          <div><div style="font-weight:700">Clear all data</div><div class="text-mute" style="font-size:12px">Delete all entries permanently</div></div>
          <button class="btn btn-danger btn-sm" id="clear-all">Clear</button>
        </div>
      </div>
    </div>
  `;
}

function emptyState(title, text) {
  return `
    <div class="empty">
      <div class="empty-icon">${I.empty}</div>
      <div class="empty-title">${title}</div>
      <div class="empty-text">${text}</div>
    </div>
  `;
}

/* ---------- Bind ---------- */
function bindPage() {
  const host = document.getElementById('page-host');

  // Quick action tiles
  host.querySelectorAll('[data-action]').forEach(b => {
    b.onclick = () => handleAction(b.dataset.action);
  });

  if (state.page === 'ledger') {
    const inp = host.querySelector('#search-inp');
    if (inp) {
      inp.oninput = debounce(() => { state.search = inp.value; renderPage(); restoreFocus('#search-inp'); }, 200);
    }
    host.querySelectorAll('[data-filter]').forEach(c => c.onclick = () => { state.filter = c.dataset.filter; renderPage(); });
    host.querySelectorAll('.entry-card').forEach(card => {
      card.onclick = () => openEntryDetail(card.dataset.id);
    });
  }

  if (state.page === 'bill') initBillBuilder();

  if (state.page === 'reports') {
    host.querySelectorAll('[data-range]').forEach(c => c.onclick = () => { state.reportRange = c.dataset.range; renderPage(); });
  }

  if (state.page === 'tools') {
    host.querySelector('#li-calc').onclick = calcLoan;
    host.querySelector('#clear-all').onclick = () => confirmDialog('Clear all data?', 'This cannot be undone.', () => {
      state.entries = []; saveData(); toast('All data cleared'); renderPage();
    });
  }
}
function restoreFocus(sel) {
  const el = document.querySelector(sel); if (el) { el.focus(); el.setSelectionRange(el.value.length, el.value.length); }
}
function debounce(fn, ms) { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; }

/* ---------- Bill builder (used both as standalone page and modal) ---------- */
let billItems = [{ name:'', qty:1, price:0 }];

function initBillBuilder() {
  billItems = [{ name:'', qty:1, price:0 }];
  renderBillItems();
  document.querySelector('#add-item').onclick = () => { billItems.push({ name:'', qty:1, price:0 }); renderBillItems(); };
  document.querySelector('#bill-paid-save').onclick = () => saveBill('paid');
  document.querySelector('#bill-udhar-save').onclick = () => saveBill('pending');
  document.querySelector('#bill-whatsapp').onclick = sendWhatsApp;
}
function renderBillItems() {
  const host = document.querySelector('#bill-items');
  host.innerHTML = billItems.map((it, i) => `
    <div class="item-row">
      <input class="input" placeholder="Item name" data-i="${i}" data-k="name" value="${escapeHtml(it.name)}" />
      <input class="input" placeholder="Qty" type="number" inputmode="numeric" data-i="${i}" data-k="qty" value="${it.qty}" />
      <input class="input" placeholder="Price" type="number" inputmode="numeric" data-i="${i}" data-k="price" value="${it.price||''}" />
      <button class="remove-btn" data-rm="${i}" title="Remove">${I.trash}</button>
    </div>
  `).join('');
  host.querySelectorAll('input').forEach(inp => {
    inp.oninput = () => {
      const i = +inp.dataset.i, k = inp.dataset.k;
      billItems[i][k] = k === 'name' ? inp.value : (+inp.value || 0);
      updateBillTotal();
    };
  });
  host.querySelectorAll('[data-rm]').forEach(b => b.onclick = () => {
    if (billItems.length === 1) { billItems = [{ name:'', qty:1, price:0 }]; }
    else billItems.splice(+b.dataset.rm, 1);
    renderBillItems();
  });
  updateBillTotal();
}
function billTotal() { return billItems.reduce((a,b) => a + (b.qty||0)*(b.price||0), 0); }
function updateBillTotal() { document.querySelector('#bill-total').textContent = fmt(billTotal()); }

function saveBill(status) {
  const name = document.querySelector('#bill-name').value.trim();
  const phone = document.querySelector('#bill-phone').value.trim();
  if (!name) return toast('Customer name required', 'error');
  const items = billItems.filter(i => i.name.trim() && i.qty > 0 && i.price > 0);
  if (!items.length) return toast('Add at least one valid item', 'error');
  const total = items.reduce((a,b) => a + b.qty*b.price, 0);
  const e = { id: uid(), name, phone, items, total, status, date: new Date().toISOString(), paidAt: status==='paid'?Date.now():null };
  state.entries.push(e); saveData();
  toast(status==='paid' ? 'Bill saved as paid' : 'Udhar entry created');
  state.page = 'dashboard'; renderShell();
}

function sendWhatsApp() {
  const name = document.querySelector('#bill-name').value.trim();
  const phone = document.querySelector('#bill-phone').value.trim();
  const items = billItems.filter(i => i.name.trim() && i.qty > 0 && i.price > 0);
  if (!items.length) return toast('Add items first', 'error');
  const text = buildBillText(name || 'Customer', items, items.reduce((a,b)=>a+b.qty*b.price,0));
  const url = phone && /^\d{10}$/.test(phone)
    ? `https://wa.me/91${phone}?text=${encodeURIComponent(text)}`
    : `https://wa.me/?text=${encodeURIComponent(text)}`;
  window.open(url, '_blank');
}
function buildBillText(name, items, total) {
  const lines = [
    `🧾 *Bill from ${state.user.name}*`,
    `Customer: ${name}`,
    `Date: ${new Date().toLocaleDateString('en-IN')}`,
    '',
    '*Items:*',
    ...items.map(i => `• ${i.name} × ${i.qty} = ₹${i.qty*i.price}`),
    '',
    `*Total: ₹${total}*`,
    '',
    '_Generated via Bahi_'
  ];
  return lines.join('\n');
}

/* ---------- Entry detail (sheet) ---------- */
function openEntryDetail(id) {
  const e = state.entries.find(x => x.id === id); if (!e) return;
  const itemsHtml = e.items.map(i => `<div class="detail-row"><div class="detail-label">${escapeHtml(i.name)} × ${i.qty}</div><div class="detail-value">${fmt(i.qty*i.price)}</div></div>`).join('');
  const m = openModal(`
    <div class="row" style="gap:12px">
      <div class="entry-avatar">${initials(e.name)}</div>
      <div style="flex:1"><div style="font-weight:800;font-size:18px">${escapeHtml(e.name)}</div>
        <div class="text-mute" style="font-size:13px">${e.phone || 'No phone'} · ${new Date(e.date).toLocaleDateString('en-IN',{day:'2-digit',month:'short',year:'numeric'})}</div>
      </div>
    </div>
    <div class="divider"></div>
    ${itemsHtml}
    <div class="detail-row" style="border-top:1px solid var(--border);margin-top:6px">
      <div style="font-weight:800">Total</div>
      <div style="font-weight:800;color:var(--primary);font-size:18px">${fmt(e.total)}</div>
    </div>
    <div class="row mt-16">
      ${e.status === 'pending' ? `<button class="btn btn-primary btn-block" id="mark-paid">${I.check}<span>Mark as Paid</span></button>` : `<span class="badge badge-paid" style="margin:0 auto;padding:8px 14px;font-size:12px"><span class="badge-dot"></span>Paid</span>`}
    </div>
    <div class="row mt-12">
      <button class="btn btn-ghost btn-block" id="wa-send">${I.whatsapp}<span style="color:inherit">WhatsApp</span></button>
      <button class="btn btn-danger btn-block" id="del">${I.trash}<span>Delete</span></button>
    </div>
  `);
  if (e.status === 'pending') m.querySelector('#mark-paid').onclick = () => {
    e.status = 'paid'; e.paidAt = Date.now(); saveData(); closeModal(); toast('Marked as paid 🎉'); renderPage();
  };
  m.querySelector('#wa-send').onclick = () => {
    const text = buildBillText(e.name, e.items, e.total);
    const url = e.phone && /^\d{10}$/.test(e.phone)
      ? `https://wa.me/91${e.phone}?text=${encodeURIComponent(text)}`
      : `https://wa.me/?text=${encodeURIComponent(text)}`;
    window.open(url, '_blank');
  };
  m.querySelector('#del').onclick = () => confirmDialog('Delete entry?', 'This action cannot be undone.', () => {
    state.entries = state.entries.filter(x => x.id !== id); saveData();
    closeModal(); toast('Entry deleted'); renderPage();
  });
}

/* ---------- Quick add modal (FAB) ---------- */
function openEntryModal() {
  state.page = 'bill'; renderShell();
}

/* ---------- Loan calc ---------- */
function calcLoan() {
  const p = +document.querySelector('#li-p').value;
  const r = +document.querySelector('#li-r').value;
  const t = +document.querySelector('#li-t').value;
  if (!p || !r || !t) return toast('Fill all fields', 'error');
  const interest = (p * r * t) / 100;
  const total = p + interest;
  document.querySelector('#li-result').innerHTML = `
    <div class="result-block">
      <div class="label">Total Repayable</div>
      <div class="value">${fmt(total)}</div>
      <div class="sub">Interest: ${fmt(interest)} · Principal: ${fmt(p)}</div>
    </div>
  `;
}

/* ---------- Actions ---------- */
function handleAction(a) {
  if (a === 'new-udhar' || a === 'new-bill') { state.page = 'bill'; renderShell(); return; }
  if (a === 'export-json') exportJSON();
  if (a === 'export-csv') exportCSV();
  if (a === 'import-json') importJSON();
}

function exportJSON() {
  const blob = new Blob([JSON.stringify({ user: state.user.name, entries: state.entries, exportedAt: new Date().toISOString() }, null, 2)], { type:'application/json' });
  download(blob, `bahi-backup-${todayKey()}.json`);
  toast('Backup downloaded');
}
function exportCSV() {
  if (!state.entries.length) return toast('No data to export', 'error');
  const rows = [['Date','Name','Phone','Items','Total','Status']];
  state.entries.forEach(e => rows.push([
    e.date.slice(0,10), e.name, e.phone||'',
    e.items.map(i => `${i.name} x${i.qty} @${i.price}`).join('; '),
    e.total, e.status
  ]));
  const csv = rows.map(r => r.map(c => `"${String(c).replace(/"/g,'""')}"`).join(',')).join('\n');
  download(new Blob([csv], { type:'text/csv' }), `bahi-export-${todayKey()}.csv`);
  toast('CSV downloaded');
}
function download(blob, name) {
  const url = URL.createObjectURL(blob);
  const a = document.createElement('a'); a.href = url; a.download = name; a.click();
  setTimeout(() => URL.revokeObjectURL(url), 1500);
}
function importJSON() {
  const inp = document.createElement('input'); inp.type = 'file'; inp.accept = 'application/json';
  inp.onchange = () => {
    const f = inp.files[0]; if (!f) return;
    const r = new FileReader();
    r.onload = () => {
      try {
        const data = JSON.parse(r.result);
        if (!Array.isArray(data.entries)) throw 0;
        confirmDialog('Restore data?', `Replace current data with ${data.entries.length} entries from backup?`, () => {
          state.entries = data.entries; saveData(); toast('Data restored'); renderPage();
        });
      } catch { toast('Invalid backup file', 'error'); }
    };
    r.readAsText(f);
  };
  inp.click();
}

/* ---------- Utils ---------- */
function escapeHtml(s) { return String(s||'').replace(/[&<>"']/g, c => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'})[c]); }

/* ---------- Boot ---------- */
function render() {
  if (state.user) renderShell();
  else renderAuth();
}
(function init() {
  applyTheme(get(DB.THEME, window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light'));
  const u = loadSession();
  if (u) { state.user = u; loadData(); }
  render();
})();
