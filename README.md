* { box-sizing: border-box; }
html, body, #root { margin: 0; min-height: 100%; }
body {
  font-family: 'Inter', 'Segoe UI', sans-serif;
  background: #f4f6fb;
  color: #20232f;
}
button, input, select { font: inherit; }
button { cursor: pointer; }
input, select {
  width: 100%;
  border: 1px solid #e1e5ef;
  border-radius: 12px;
  padding: 11px 12px;
  background: white;
  color: #1f2430;
}
input:focus, select:focus { outline: 2px solid rgba(88, 106, 229, 0.15); border-color: #7d86ee; }

.auth-shell {
  min-height: 100vh;
  display: grid;
  place-items: center;
  padding: 24px;
  background: linear-gradient(135deg, #f3f5ff 0%, #eef9f5 100%);
}

.auth-card {
  width: min(100%, 480px);
  background: rgba(255, 255, 255, 0.85);
  border: 1px solid rgba(129, 138, 178, 0.14);
  border-radius: 28px;
  box-shadow: 0 30px 80px rgba(39, 48, 94, 0.12);
  padding: 28px 24px;
  backdrop-filter: blur(14px);
}

.brand-block {
  display: flex;
  align-items: center;
  gap: 16px;
  margin-bottom: 18px;
}

.brand-mark {
  width: 42px;
  height: 42px;
  border-radius: 14px;
  display: grid;
  place-items: center;
  font-weight: 800;
  color: white;
  background: linear-gradient(135deg, #646fe8 0%, #4c59d4 100%);
  box-shadow: 0 18px 36px rgba(100, 111, 232, 0.28);
}

.brand-block h1 {
  margin: 0;
  font-size: 2rem;
  letter-spacing: -0.08em;
}

.brand-block p {
  margin: 4px 0 0;
  color: #757e95;
  font-size: 0.9rem;
}

.auth-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 12px;
  margin-bottom: 18px;
}

.toggle-group {
  display: flex;
  background: #f3f4f9;
  border-radius: 12px;
  padding: 4px;
  gap: 4px;
}

.toggle-group button {
  border: none;
  background: transparent;
  color: #5f6475;
  padding: 8px 12px;
  border-radius: 10px;
  font-size: 0.85rem;
  font-weight: 600;
}

.toggle-group button.active {
  background: white;
  color: #1d2435;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.05);
}

.auth-form {
  display: flex;
  flex-direction: column;
  gap: 14px;
}

.auth-form label {
  display: flex;
  flex-direction: column;
  gap: 8px;
  color: #4d5568;
  font-size: 0.78rem;
  font-weight: 600;
}

.primary-btn, .secondary-btn, .mini-btn, .icon-btn, .logout-btn, .nav-item, .text-button {
  transition: all 0.18s ease;
}

.primary-btn {
  border: none;
  border-radius: 12px;
  background: linear-gradient(135deg, #5b68e7 0%, #4a58d2 100%);
  color: white;
  padding: 12px 16px;
  font-weight: 700;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  box-shadow: 0 16px 30px rgba(88, 106, 229, 0.24);
}

.secondary-btn {
  border: 1px solid #e7eaf5;
  background: white;
  color: #2a3143;
  padding: 12px 14px;
  border-radius: 12px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  font-weight: 600;
}

.app-shell {
  display: flex;
  min-height: 100vh;
  background: #f4f6fb;
}

.sidebar {
  width: 250px;
  background: rgba(255, 255, 255, 0.7);
  border-right: 1px solid rgba(196, 201, 214, 0.7);
  padding: 22px 16px 18px;
  backdrop-filter: blur(12px);
  display: flex;
  flex-direction: column;
}

.brand-row {
  display: flex;
  align-items: center;
  gap: 12px;
  margin-bottom: 24px;
  padding: 0 6px;
}

.brand-row .brand-mark { width: 34px; height: 34px; }
.brand-name {
  font-weight: 800;
  letter-spacing: -0.07em;
  font-size: 1.2rem;
}
.brand-row small {
  display: block;
  color: #7d8394;
  font-size: 0.72rem;
}

.nav {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.nav-item {
  border: none;
  background: transparent;
  color: #5d6374;
  border-radius: 12px;
  padding: 10px 12px;
  display: flex;
  align-items: center;
  gap: 10px;
  text-align: left;
  font-weight: 600;
}

.nav-item.active {
  background: linear-gradient(135deg, rgba(90, 103, 231, 0.12), rgba(90, 103, 231, 0.05));
  color: #4654d2;
}

.profile-card {
  margin-top: auto;
  display: flex;
  align-items: center;
  gap: 12px;
  background: #f9faff;
  border: 1px solid #edf0f7;
  border-radius: 16px;
  padding: 12px 10px;
}

.avatar {
  width: 34px;
  height: 34px;
  border-radius: 50%;
  background: linear-gradient(135deg, #e3e7ff 0%, #d5d8ff 100%);
  color: #4654d2;
  display: grid;
  place-items: center;
  font-weight: 700;
}

.profile-card strong {
  display: block;
  font-size: 0.76rem;
}

.profile-card small {
  display: block;
  color: #7c8292;
  font-size: 0.7rem;
}

.logout-btn {
  border: none;
  background: transparent;
  color: #5d6374;
  padding: 12px 10px 0;
  display: flex;
  align-items: center;
  gap: 8px;
  font-weight: 600;
}

.main-panel {
  flex: 1;
  min-width: 0;
}

.topbar {
  height: 72px;
  background: rgba(255, 255, 255, 0.72);
  border-bottom: 1px solid rgba(196, 201, 214, 0.7);
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 28px;
  position: sticky;
  top: 0;
  z-index: 2;
  backdrop-filter: blur(12px);
}

.date-pill {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  font-weight: 600;
  font-size: 0.82rem;
  color: #4e5568;
}

.top-actions {
  display: flex;
  align-items: center;
  gap: 12px;
}

.top-actions select {
  width: auto;
  min-width: 120px;
}

.content-wrap {
  max-width: 1200px;
  margin: 0 auto;
  padding: 26px 28px 40px;
}

.row {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 16px;
  margin-bottom: 18px;
}

.eyebrow {
  color: #7b8092;
  font-size: 0.72rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  font-weight: 700;
}

h1, h2, h3, p { margin: 0; }
h1 {
  margin-top: 6px;
  font-size: clamp(2rem, 3vw, 2.7rem);
  letter-spacing: -0.08em;
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 14px;
  margin-bottom: 18px;
}

.stats-grid.three {
  grid-template-columns: repeat(3, minmax(0, 1fr));
}

.stat-card {
  background: white;
  border: 1px solid #edf0f7;
  border-radius: 18px;
  padding: 16px 18px;
  box-shadow: 0 8px 22px rgba(15, 23, 42, 0.03);
}

.stat-icon {
  width: 36px;
  height: 36px;
  border-radius: 12px;
  display: grid;
  place-items: center;
  margin-bottom: 14px;
}

.stat-icon.green { background: #ebfaf1; color: #2a9f67; }
.stat-icon.red { background: #fff0f1; color: #d45d68; }
.stat-icon.blue { background: #edf1ff; color: #5368db; }
.stat-icon.purple { background: #f6efff; color: #8c5fe0; }

.stat-label {
  color: #7a7e8f;
  font-size: 0.72rem;
}

.stat-card strong {
  display: block;
  margin-top: 6px;
  font-size: 1.2rem;
  letter-spacing: -0.06em;
}

.two-col {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 14px;
  margin-bottom: 18px;
}

.panel {
  background: white;
  border-radius: 20px;
  border: 1px solid #edf0f7;
  padding: 18px 18px 12px;
  box-shadow: 0 10px 26px rgba(15, 23, 42, 0.025);
}

.panel-head {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 10px;
  margin-bottom: 12px;
}

.panel-head h3 { font-size: 1rem; }

.mini-btn {
  border: none;
  background: #f3f4fb;
  color: #5560c8;
  border-radius: 10px;
  padding: 7px 10px;
  font-size: 0.75rem;
  font-weight: 600;
}

.empty-box {
  display: grid;
  place-items: center;
  text-align: center;
  padding: 18px 8px 8px;
  color: #7d8395;
  min-height: 140px;
}

.empty-box p {
  margin-top: 10px;
  font-size: 0.85rem;
}

.empty-icon {
  width: 42px;
  height: 42px;
  border-radius: 12px;
  display: grid;
  place-items: center;
  background: #f3f5ff;
  color: #5a69d8;
}

.stack-list {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.stack-row {
  display: flex;
  align-items: center;
  gap: 10px;
  border-top: 1px solid #eef0f5;
  padding-top: 10px;
}

.stack-row:first-child { border-top: none; padding-top: 0; }

.stack-row.done .stack-main strong { text-decoration: line-through; color: #8b91a3; }

.check-btn {
  width: 20px;
  height: 20px;
  border-radius: 6px;
  border: 1px solid #dfe5f2;
  background: white;
  display: grid;
  place-items: center;
  color: white;
}

.check-btn.done {
  background: #38b67b;
  border-color: #38b67b;
}

.stack-main {
  flex: 1;
  min-width: 0;
}

.stack-main strong {
  display: block;
  font-size: 0.87rem;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.stack-main small {
  display: block;
  color: #8a8fa0;
  font-size: 0.72rem;
  margin-top: 2px;
}

.badge {
  border-radius: 999px;
  background: #f3f4fb;
  color: #5d6374;
  font-size: 0.68rem;
  padding: 6px 8px;
  white-space: nowrap;
}

.icon-btn {
  border: 1px solid #edf0f7;
  background: white;
  color: #5b6073;
  width: 30px;
  height: 30px;
  border-radius: 10px;
  display: grid;
  place-items: center;
}

.icon-btn.small {
  width: 26px;
  height: 26px;
}

.tx-icon {
  width: 32px;
  height: 32px;
  border-radius: 10px;
  display: grid;
  place-items: center;
}

.tx-icon.income { background: #ebfaf1; color: #2b9b67; }
.tx-icon.expense { background: #fff0f1; color: #d55d6a; }

.money {
  font-size: 0.8rem;
  font-weight: 700;
  white-space: nowrap;
}

.money.income { color: #2e9f69; }
.money.expense { color: #d15d68; }

.month-switcher {
  display: flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 18px;
}

.month-switcher strong {
  min-width: 130px;
  text-align: center;
  font-size: 0.9rem;
  text-transform: capitalize;
}

.month-switcher input {
  width: 120px;
}

.report-box {
  margin-top: 12px;
}

.report-head {
  display: flex;
  align-items: center;
  gap: 12px;
  margin-bottom: 20px;
}

.report-head h3 { font-size: 1.05rem; }
.report-head small { color: #81879a; }

.spark {
  width: 36px;
  height: 36px;
  background: linear-gradient(135deg, #f0f3ff 0%, #e8f9f0 100%);
  color: #5d68e7;
  border-radius: 12px;
  display: grid;
  place-items: center;
}

.report-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 14px;
}

.report-grid div {
  background: #f9fafc;
  border: 1px solid #eef1f7;
  border-radius: 14px;
  padding: 12px 14px;
}

.report-grid span {
  display: block;
  font-size: 0.68rem;
  color: #7d8292;
  margin-bottom: 6px;
}

.report-grid strong {
  font-size: 0.95rem;
  letter-spacing: -0.03em;
}

.goal-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 14px;
}

.goal-card {
  position: relative;
}

.goal-top {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 12px;
}

.goal-icon {
  width: 36px;
  height: 36px;
  border-radius: 12px;
  background: #edf1ff;
  color: #5467de;
  display: grid;
  place-items: center;
}

.goal-card h3 {
  font-size: 1rem;
  margin-bottom: 8px;
}

.goal-amount {
  font-weight: 700;
  letter-spacing: -0.04em;
  margin-bottom: 12px;
}

.progress-track {
  width: 100%;
  height: 8px;
  border-radius: 999px;
  background: #eef1f7;
  overflow: hidden;
  margin-bottom: 10px;
}

.progress-track span {
  display: block;
  height: 100%;
  background: linear-gradient(90deg, #6170e3 0%, #7e89e6 100%);
  border-radius: inherit;
}

.goal-bottom {
  display: flex;
  justify-content: space-between;
  color: #7d8394;
  font-size: 0.72rem;
}

.empty-panel {
  min-height: 180px;
  display: grid;
  place-items: center;
  text-align: center;
}

.search-head {
  align-items: center;
}

.search-box {
  display: flex;
  align-items: center;
  gap: 8px;
  border: 1px solid #edf0f7;
  border-radius: 10px;
  padding: 7px 10px;
  background: #fafbfd;
  width: 160px;
}

.search-box input {
  border: none;
  background: transparent;
  padding: 0;
  width: 100%;
}

.settings-panel {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 14px;
}

.settings-panel strong {
  display: block;
  margin-bottom: 4px;
}

.settings-panel small {
  color: #7d8395;
}

.settings-panel select {
  width: 150px;
}

.note-box {
  display: flex;
  align-items: flex-start;
  gap: 12px;
  color: #697184;
  line-height: 1.6;
}

.note-box p { font-size: 0.82rem; }

.modal-backdrop {
  position: fixed;
  inset: 0;
  background: rgba(31, 36, 48, 0.35);
  display: grid;
  place-items: center;
  padding: 16px;
  z-index: 30;
}

.modal {
  width: min(460px, 100%);
  background: white;
  border: 1px solid #eef0f7;
  border-radius: 20px;
  box-shadow: 0 30px 70px rgba(17, 20, 33, 0.22);
  padding: 18px 18px 14px;
}

.modal-head {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 12px;
}

.modal label {
  display: flex;
  flex-direction: column;
  gap: 8px;
  margin-bottom: 12px;
  color: #5b6376;
  font-size: 0.76rem;
  font-weight: 600;
}

.two-fields {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 10px;
}

.modal-actions {
  display: flex;
  justify-content: flex-end;
  gap: 10px;
  margin-top: 8px;
}

@media (max-width: 980px) {
  .two-col { grid-template-columns: 1fr; }
  .goal-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
}

@media (max-width: 820px) {
  .app-shell { display: block; }
  .sidebar {
    width: 100%;
    border-right: none;
    border-bottom: 1px solid rgba(196, 201, 214, 0.7);
    padding: 16px 12px 12px;
  }
  .brand-row { margin-bottom: 12px; }
  .nav {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 8px;
  }
  .profile-card { margin-top: 12px; }
  .main-panel { min-height: auto; }
  .content-wrap { padding: 20px 16px 30px; }
  .topbar { padding: 0 16px; }
}

@media (max-width: 640px) {
  .stats-grid, .stats-grid.three { grid-template-columns: 1fr 1fr; }
  .goal-grid { grid-template-columns: 1fr; }
  .two-fields { grid-template-columns: 1fr; }
  .topbar { height: auto; min-height: 72px; padding: 14px 16px; }
  .top-actions { gap: 8px; }
  .top-actions select { min-width: 90px; }
  .month-switcher { flex-wrap: wrap; }
  .search-head { flex-direction: column; align-items: stretch; }
  .search-box { width: 100%; }
}

@media (max-width: 480px) {
  .auth-card { padding: 22px 18px; }
  .brand-block { align-items: flex-start; }
  .brand-block h1 { font-size: 1.6rem; }
  .toggle-group { width: 100%; }
  .toggle-group button { flex: 1; }
  .auth-header { flex-direction: column; align-items: stretch; }
  .stats-grid, .stats-grid.three { grid-template-columns: 1fr; }
  .row { flex-direction: column; align-items: flex-start; }
  .primary-btn { width: 100%; }
  .top-actions { width: 100%; justify-content: space-between; }
}

@media (prefers-reduced-motion: reduce) {
  * { scroll-behavior: auto !important; transition: none !important; }
}
