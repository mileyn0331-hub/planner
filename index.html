<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Daily Planner</title>
<link rel="icon" type="image/svg+xml" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 32 32'%3E%3Crect width='32' height='32' rx='8' fill='%23185FA5'/%3E%3Crect x='6' y='8' width='20' height='18' rx='3' fill='white'/%3E%3Crect x='6' y='8' width='20' height='6' rx='3' fill='%23378ADD'/%3E%3Crect x='10' y='4' width='3' height='6' rx='1.5' fill='white'/%3E%3Crect x='19' y='4' width='3' height='6' rx='1.5' fill='white'/%3E%3Crect x='9' y='18' width='5' height='2' rx='1' fill='%23378ADD'/%3E%3Crect x='9' y='21' width='8' height='2' rx='1' fill='%23B5D4F4'/%3E%3Crect x='18' y='18' width='5' height='2' rx='1' fill='%23B5D4F4'/%3E%3C/svg%3E">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@400;500;600&display=swap" rel="stylesheet">

<style>
*{box-sizing:border-box;margin:0;padding:0}
html,body{height:100%;font-family:'Noto Sans KR',sans-serif;transition:background 0.2s,color 0.2s}

:root{
  --bg-page:#F0F4F8;
  --bg-surface:#FFFFFF;
  --bg-surface2:#F8FAFB;
  --bg-surface3:#EEF2F6;
  --text-primary:#1E293B;
  --text-secondary:#475569;
  --text-muted:#94A3B8;
  --border:#E2E8F0;
  --border-hover:#94A3B8;
  --blue-50:#E6F1FB;--blue-100:#B5D4F4;--blue-200:#85B7EB;
  --blue-400:#378ADD;--blue-600:#185FA5;--blue-800:#0C447C;--blue-900:#042C53;
  --block-empty:#EEF2F6;
  --block-empty-border:#E2E8F0;
  --block-hover-bg:#dbeafe;
  --block-hover-border:#93c5fd;
  --radius-sm:6px;--radius-md:10px;--radius-lg:14px;
  --shadow-sm:0 1px 3px rgba(0,0,0,0.07),0 1px 2px rgba(0,0,0,0.05);
  --shadow-md:0 4px 16px rgba(0,0,0,0.10),0 2px 4px rgba(0,0,0,0.06);
  --shadow-lg:0 8px 32px rgba(0,0,0,0.14),0 2px 8px rgba(0,0,0,0.08);
}

[data-theme="dark"]{
  --bg-page:#0F172A;
  --bg-surface:#1E293B;
  --bg-surface2:#162032;
  --bg-surface3:#253347;
  --text-primary:#F1F5F9;
  --text-secondary:#E2E8F0;
  --text-muted:#64748B;
  --border:#2D3F55;
  --border-hover:#4A6080;
  --blue-50:#0c2340;--blue-100:#0e3460;--blue-200:#1a4f8a;
  --blue-400:#378ADD;--blue-600:#4E9FE5;--blue-800:#85B7EB;--blue-900:#B5D4F4;
  --block-empty:#1E2D3D;
  --block-empty-border:#2D3F55;
  --block-hover-bg:#1a3a5c;
  --block-hover-border:#378ADD;
}

body{background:var(--bg-page);color:var(--text-primary)}

/* ── VIEWS ── */
#plannerView{width:100%;height:100vh}
#calendarView{display:none;width:100%;height:100vh;flex-direction:column;background:var(--bg-page);position:fixed;top:0;left:0;z-index:50}
#calendarView.active{display:flex}
#plannerView.hidden{display:none}

/* ── PLANNER LAYOUT ── */
.app{
  display:grid;
  grid-template-columns:260px 1fr 1fr;
  grid-template-rows:56px 1fr;
  height:100vh;
  min-width:820px;
}

/* ── TOP BAR ── */
.topbar{
  grid-column:1/-1;
  background:var(--bg-surface);
  border-bottom:1px solid var(--border);
  display:flex;align-items:center;
  padding:0 20px;gap:12px;
  box-shadow:var(--shadow-sm);z-index:10;
}
.topbar-logo{
  font-size:15px;font-weight:600;color:var(--blue-600);
  letter-spacing:-0.02em;display:flex;align-items:center;gap:7px;flex-shrink:0;
}
.topbar-logo i{font-size:18px;color:var(--blue-400)}
.topbar-divider{width:1px;height:20px;background:var(--border);margin:0 2px;flex-shrink:0}
.date-display-static{
  font-size:14px;font-weight:500;color:var(--text-primary);
}
.today-pill{
  font-size:11px;font-weight:500;background:var(--blue-50);color:var(--blue-600);
  border-radius:20px;padding:2px 10px;border:1px solid var(--blue-100);flex-shrink:0;
}
.topbar-right{margin-left:auto;display:flex;align-items:center;gap:7px}
.tb-btn{
  height:30px;padding:0 11px;
  font-size:12px;font-weight:500;font-family:inherit;
  background:var(--bg-surface);border:1px solid var(--border);
  border-radius:var(--radius-sm);cursor:pointer;
  color:var(--text-secondary);
  display:flex;align-items:center;gap:5px;
  transition:all 0.15s;white-space:nowrap;
}
.tb-btn:hover{border-color:var(--border-hover);color:var(--text-primary);background:var(--bg-surface2)}
.tb-btn.active{background:var(--blue-50);border-color:var(--blue-200);color:var(--blue-600)}
[data-theme="dark"] .tb-btn.active{background:var(--blue-50);border-color:var(--blue-200);color:var(--blue-800)}

/* view mode */
body.view-mode .block{cursor:default !important;pointer-events:none}
body.view-mode .schedule-del{pointer-events:none;opacity:0}
body.view-mode .todo-input-row{opacity:0.4;pointer-events:none}
body.view-mode #viewModeBtn{background:var(--blue-50);border-color:var(--blue-400);color:var(--blue-600);font-weight:600}
body.view-mode .topbar{border-bottom:2px solid var(--blue-400)}

/* ── PANELS ── */
.panel{
  background:var(--bg-surface);border-right:1px solid var(--border);
  display:flex;flex-direction:column;overflow:hidden;
}
.panel:last-child{border-right:none}
.panel-header{
  padding:13px 16px 11px;border-bottom:1px solid var(--border);
  flex-shrink:0;background:var(--bg-surface);
}
.panel-title{
  font-size:11px;font-weight:600;color:var(--text-muted);
  text-transform:uppercase;letter-spacing:0.08em;
}
.panel-body{flex:1;overflow-y:auto;padding:12px}
.panel-body::-webkit-scrollbar{width:4px}
.panel-body::-webkit-scrollbar-track{background:transparent}
.panel-body::-webkit-scrollbar-thumb{background:var(--border);border-radius:2px}

/* ── BLOCK GRID ── */
.time-label-row{
  display:grid;grid-template-columns:36px repeat(6,1fr);
  gap:2px;margin-bottom:5px;
}
.time-col-label{font-size:9px;font-weight:500;color:var(--text-muted);text-align:center;letter-spacing:0.04em}
.block-grid{display:flex;flex-direction:column;gap:2px;user-select:none}
.block-row{display:grid;grid-template-columns:36px repeat(6,1fr);gap:2px;align-items:center}
.row-hour-label{
  font-size:10px;color:var(--text-muted);text-align:right;padding-right:6px;
  font-variant-numeric:tabular-nums;line-height:1;flex-shrink:0;
}
.block{
  height:20px;border-radius:3px;
  background:var(--block-empty);border:1px solid var(--block-empty-border);
  cursor:pointer;transition:background 0.08s,border-color 0.08s,opacity 0.08s;
  position:relative;
}
.block:hover{border-color:var(--block-hover-border);background:var(--block-hover-bg)}
.block.filled{border:none;opacity:0.85}
.block.filled:hover{opacity:1}
.block.kb-focus{
  outline:2px solid var(--blue-600) !important;
  outline-offset:-2px;
  z-index:2;
}
.block.kb-range{
  outline:2px solid var(--blue-400) !important;
  outline-offset:-2px;
  background:var(--block-hover-bg);
}
/* drag-select preview highlight */
.block.drag-preview{
  outline:2px solid var(--blue-400);
  outline-offset:-1px;
  opacity:0.7;
}
/* current time block highlight */
.block.now-block{
  outline:2px solid #EF9F27 !important;
  outline-offset:-2px;
}
/* erasing mode: red tint on hover */
.block.filled:not(.schedule-block):hover{
  outline:2px solid #E24B4A;outline-offset:-1px;
}
/* todo keyboard focus */
.todo-item.kb-focus{
  outline:2px solid var(--blue-400);
  outline-offset:-2px;
  background:var(--bg-surface2);
}
.todo-item.selected{
  background:var(--blue-50);
  border-color:var(--blue-200);
}
/* schedule item keyboard focus */
.schedule-item.kb-focus{
  outline:2px solid var(--blue-400);
  outline-offset:-2px;
}
/* shortcut help overlay */
.shortcut-overlay{
  position:fixed;inset:0;background:rgba(15,23,42,0.55);
  display:flex;align-items:center;justify-content:center;
  z-index:2000;opacity:0;pointer-events:none;transition:opacity 0.2s;
}
.shortcut-overlay.open{opacity:1;pointer-events:auto}
.shortcut-box{
  background:var(--bg-surface);border:1px solid var(--border);
  border-radius:var(--radius-lg);padding:20px 22px;
  min-width:340px;max-width:420px;width:90%;
  box-shadow:0 20px 60px rgba(0,0,0,0.2);
}
.shortcut-box h3{font-size:14px;font-weight:600;color:var(--text-primary);margin-bottom:14px;display:flex;align-items:center;justify-content:space-between}
.shortcut-close-btn{background:none;border:none;cursor:pointer;color:var(--text-muted);font-size:16px;padding:0;line-height:1;transition:color 0.15s}
.shortcut-close-btn:hover{color:var(--text-primary)}
/* accordion */
.sc-cat{border:1px solid var(--border);border-radius:var(--radius-md);margin-bottom:6px;overflow:hidden}
.sc-cat:last-child{margin-bottom:0}
.sc-cat-btn{
  width:100%;display:flex;align-items:center;justify-content:space-between;
  padding:9px 12px;background:var(--bg-surface2);border:none;cursor:pointer;
  font-size:12px;font-weight:600;color:var(--text-secondary);font-family:inherit;
  text-transform:uppercase;letter-spacing:0.07em;transition:background 0.15s;
}
.sc-cat-btn:hover{background:var(--bg-surface3);color:var(--text-primary)}
.sc-cat-btn .sc-arrow{font-size:10px;transition:transform 0.2s;color:var(--text-muted)}
.sc-cat.open .sc-cat-btn .sc-arrow{transform:rotate(180deg)}
.sc-cat-body{display:none;padding:8px 12px;border-top:1px solid var(--border)}
.sc-cat.open .sc-cat-body{display:block}
.shortcut-row{display:flex;align-items:center;justify-content:space-between;padding:4px 0;font-size:12px;color:var(--text-secondary)}
kbd{
  display:inline-flex;align-items:center;justify-content:center;
  background:var(--bg-surface3);border:1px solid var(--border);
  border-radius:4px;padding:1px 6px;font-size:11px;font-family:inherit;
  color:var(--text-primary);min-width:22px;
}

/* ── SCHEDULE PANEL ── */
.schedule-list{display:flex;flex-direction:column;gap:6px}
.schedule-item{
  display:flex;align-items:stretch;
  background:var(--bg-surface);border:1px solid var(--border);
  border-radius:var(--radius-md);overflow:hidden;transition:box-shadow 0.15s;
}
.schedule-item:hover{box-shadow:var(--shadow-sm)}
.schedule-bookmark{width:5px;flex-shrink:0}
.schedule-content{flex:1;padding:8px 10px;min-width:0}
.schedule-title{font-size:13px;font-weight:500;color:var(--text-primary);margin-bottom:2px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.schedule-time-tag{font-size:11px;color:var(--text-muted);display:flex;align-items:center;gap:4px}
.schedule-del{
  background:none;border:none;cursor:pointer;color:var(--text-muted);
  padding:0 10px;display:flex;align-items:center;justify-content:center;
  transition:color 0.15s,background 0.15s;font-size:14px;
}
.schedule-del:hover{color:var(--text-secondary);background:var(--bg-surface2)}

/* memo ref banner */
.memo-ref-banner{
  background:var(--blue-50);border:1px solid var(--blue-100);
  border-radius:var(--radius-md);padding:8px 11px;margin-bottom:8px;
}
.memo-ref-title{font-size:10px;font-weight:600;color:var(--blue-600);letter-spacing:0.06em;text-transform:uppercase;margin-bottom:5px}
.memo-ref-item{font-size:12px;color:var(--blue-800);display:flex;align-items:center;gap:5px;padding:1px 0}
[data-theme="dark"] .memo-ref-banner{background:var(--blue-50)}
[data-theme="dark"] .memo-ref-title{color:var(--blue-800)}
[data-theme="dark"] .memo-ref-item{color:var(--blue-900)}

/* ── TODO ── */
.todo-input-row{
  padding:12px 14px;border-bottom:1px solid var(--border);
  display:flex;gap:6px;background:var(--bg-surface2);flex-shrink:0;
}
.todo-list{display:flex;flex-direction:column;gap:4px}
.todo-item{
  display:flex;align-items:center;gap:9px;padding:8px 10px;
  background:var(--bg-surface);border:1px solid var(--border);
  border-radius:var(--radius-md);cursor:pointer;transition:all 0.15s;
}
.todo-item:hover{background:var(--bg-surface2)}
.todo-item:hover .todo-check{color:var(--blue-400)}
.todo-check{color:var(--border-hover);font-size:17px;transition:color 0.15s;flex-shrink:0}
.todo-text{font-size:13px;color:var(--text-secondary);flex:1;line-height:1.4}

.section-lbl{font-size:11px;font-weight:600;color:var(--text-muted);text-transform:uppercase;letter-spacing:0.07em;margin:10px 0 6px;padding:0 2px}
.empty-hint{font-size:12px;color:var(--text-muted);text-align:center;padding:20px 0}

/* ── INPUTS ── */
input[type=text],input[type=time]{
  font-size:13px;font-family:inherit;padding:7px 10px;
  border:1px solid var(--border);border-radius:var(--radius-sm);
  background:var(--bg-surface);color:var(--text-primary);
  outline:none;width:100%;transition:border-color 0.15s,box-shadow 0.15s;
}
input[type=text]:focus,input[type=time]:focus{
  border-color:var(--blue-400);box-shadow:0 0 0 3px rgba(55,138,221,0.12);
}
.field-label{font-size:11px;font-weight:500;color:var(--text-secondary);margin-bottom:3px}
.primary-btn{
  font-size:12px;font-weight:600;font-family:inherit;padding:7px 14px;
  background:var(--blue-600);color:#fff;border:none;border-radius:var(--radius-sm);
  cursor:pointer;display:flex;align-items:center;gap:4px;
  white-space:nowrap;transition:background 0.15s;flex-shrink:0;
}
.primary-btn:hover{background:var(--blue-800)}
.primary-btn:active{transform:scale(0.98)}
[data-theme="dark"] .primary-btn{background:var(--blue-400)}
[data-theme="dark"] .primary-btn:hover{background:var(--blue-200);color:var(--bg-page)}

/* ── SCHEDULE REGISTER POPUP (drag select) ── */
.schedule-popup{
  position:fixed;z-index:500;
  background:var(--bg-surface);border:1px solid var(--border);
  border-radius:var(--radius-lg);padding:16px;width:320px;
  box-shadow:var(--shadow-lg);
  display:none;flex-direction:column;gap:10px;
}
.schedule-popup.open{display:flex}
.popup-time-range{
  font-size:11px;font-weight:600;color:var(--blue-600);
  letter-spacing:0.05em;margin-bottom:2px;
}
.color-swatches{display:grid;grid-template-columns:repeat(2,1fr);gap:4px;width:100%}
.color-btn{
  display:flex;align-items:center;gap:7px;
  padding:6px 9px;border-radius:var(--radius-sm);
  border:1.5px solid var(--border);background:var(--bg-surface);
  cursor:pointer;transition:all 0.12s;outline:none;
  font-size:12px;font-family:inherit;color:var(--text-secondary);
  white-space:nowrap;width:100%;text-align:left;
}
.color-btn:hover{border-color:var(--border-hover);background:var(--bg-surface2);color:var(--text-primary)}
.color-btn.active{background:var(--bg-surface);color:var(--text-primary);font-weight:600}
.color-btn .cb-dot{width:9px;height:9px;border-radius:50%;flex-shrink:0}
.color-btn .cb-label{font-size:11px}

/* ── MODALS ── */
.modal-overlay{
  position:fixed;inset:0;background:rgba(15,23,42,0.45);
  display:flex;align-items:center;justify-content:center;
  z-index:1000;opacity:0;pointer-events:none;transition:opacity 0.2s;
}
.modal-overlay.open{opacity:1;pointer-events:auto}
.modal{
  background:var(--bg-surface);border-radius:var(--radius-lg);
  padding:24px;max-width:340px;width:90%;
  box-shadow:0 20px 60px rgba(0,0,0,0.2);border:1px solid var(--border);
  transform:translateY(8px);transition:transform 0.2s;
}
.modal-overlay.open .modal{transform:translateY(0)}
.modal-title{font-size:15px;font-weight:600;color:var(--text-primary);margin-bottom:6px}
.modal-desc{font-size:13px;color:var(--text-secondary);margin-bottom:20px;line-height:1.5}
.modal-actions{display:flex;gap:8px;justify-content:flex-end}
.modal-cancel{
  font-size:13px;font-weight:500;font-family:inherit;padding:7px 16px;
  background:var(--bg-surface);border:1px solid var(--border);
  border-radius:var(--radius-sm);cursor:pointer;color:var(--text-secondary);transition:all 0.15s;
}
.modal-cancel:hover{border-color:var(--border-hover);color:var(--text-primary)}
.modal-confirm{
  font-size:13px;font-weight:600;font-family:inherit;padding:7px 16px;
  background:#E24B4A;color:#fff;border:none;border-radius:var(--radius-sm);cursor:pointer;
}
.modal-confirm:hover{background:#A32D2D}

/* ── CALENDAR VIEW ── */
.cal-topbar{
  background:var(--bg-surface);border-bottom:1px solid var(--border);
  display:flex;align-items:center;padding:0 24px;gap:14px;
  height:56px;flex-shrink:0;box-shadow:var(--shadow-sm);
}
.cal-back-btn{
  height:30px;padding:0 12px;font-size:13px;font-weight:500;font-family:inherit;
  background:var(--bg-surface);border:1px solid var(--border);
  border-radius:var(--radius-sm);cursor:pointer;color:var(--text-secondary);
  display:flex;align-items:center;gap:6px;transition:all 0.15s;
}
.cal-back-btn:hover{border-color:var(--border-hover);color:var(--text-primary);background:var(--bg-surface2)}
.cal-title{font-size:15px;font-weight:600;color:var(--text-primary)}
.cal-month-nav{display:flex;align-items:center;gap:8px;margin-left:auto}
.cal-month-btn{
  width:32px;height:32px;border-radius:var(--radius-sm);
  border:1px solid var(--border);background:var(--bg-surface);
  cursor:pointer;display:flex;align-items:center;justify-content:center;
  color:var(--text-primary);font-size:16px;transition:all 0.15s;
}
.cal-month-btn:hover{background:var(--bg-surface3);border-color:var(--border-hover)}
.cal-month-label{font-size:14px;font-weight:500;color:var(--text-primary);min-width:80px;text-align:center}
.cal-body{flex:1;overflow-y:auto;padding:24px}
.cal-grid-wrap{max-width:900px;margin:0 auto}
.cal-day-headers{display:grid;grid-template-columns:repeat(7,1fr);gap:6px;margin-bottom:6px}
.cal-day-hdr{font-size:11px;font-weight:600;color:var(--text-muted);text-align:center;padding:4px 0;letter-spacing:0.06em}
.cal-day-hdr.weekend{color:#E24B4A}
.cal-grid{display:grid;grid-template-columns:repeat(7,1fr);gap:6px}
.cal-cell{
  min-height:80px;border-radius:var(--radius-md);
  background:var(--bg-surface);border:1px solid var(--border);
  padding:8px 9px;cursor:pointer;transition:all 0.15s;position:relative;
}
.cal-cell:hover:not(.cal-cell-empty):not(.cal-cell-past){border-color:var(--blue-400);box-shadow:var(--shadow-sm)}
.cal-cell.kb-focus:not(.cal-cell-empty):not(.cal-cell-past){
  outline:2px solid var(--blue-600);outline-offset:-2px;
  box-shadow:var(--shadow-sm);
}
.cal-cell-empty{background:transparent;border:1px solid transparent;cursor:default}
.cal-cell-past{opacity:0.45;cursor:default}
.cal-cell-today{border-color:var(--blue-400) !important;background:var(--blue-50)}
.cal-cell-today .cal-date-num{color:var(--blue-600);font-weight:600}
.cal-date-num{font-size:13px;font-weight:500;color:var(--text-primary);margin-bottom:5px}
.cal-memo-dot{
  display:none;width:6px;height:6px;border-radius:50%;
  background:var(--blue-400);position:absolute;top:8px;right:9px;
}
.cal-cell-has-memo .cal-memo-dot{display:block}
.cal-memo-list{display:flex;flex-direction:column;gap:3px}
.cal-memo-chip{
  font-size:10px;color:var(--blue-800);background:var(--blue-100);
  border-radius:4px;padding:2px 5px;line-height:1.4;
  overflow:hidden;text-overflow:ellipsis;white-space:nowrap;
}
[data-theme="dark"] .cal-memo-chip{background:var(--blue-50);color:var(--blue-900)}

/* memo modal */
.memo-modal{
  background:var(--bg-surface);border-radius:var(--radius-lg);
  padding:22px;max-width:360px;width:90%;
  box-shadow:0 20px 60px rgba(0,0,0,0.2);border:1px solid var(--border);
  transform:translateY(8px);transition:transform 0.2s;
}
.modal-overlay.open .memo-modal{transform:translateY(0)}
.memo-modal-date{font-size:12px;font-weight:600;color:var(--blue-600);letter-spacing:0.05em;margin-bottom:4px}
.memo-modal-title{font-size:15px;font-weight:600;color:var(--text-primary);margin-bottom:14px}
.memo-modal-list{display:flex;flex-direction:column;gap:6px;margin-bottom:12px;min-height:20px}
.memo-modal-item{
  display:flex;align-items:center;gap:8px;padding:7px 10px;
  background:var(--bg-surface2);border:1px solid var(--border);border-radius:var(--radius-sm);
}
.memo-modal-text{font-size:13px;color:var(--text-primary);flex:1}
.memo-modal-del{background:none;border:none;cursor:pointer;color:var(--text-muted);font-size:13px;transition:color 0.15s;padding:2px}
.memo-modal-del:hover{color:var(--text-primary)}
.ic{display:inline-flex;align-items:center;justify-content:center;flex-shrink:0;vertical-align:middle}
.ic svg{width:1em;height:1em;stroke:currentColor;fill:none;stroke-width:1.5;stroke-linecap:round;stroke-linejoin:round}

/* ── AUTH SCREEN ── */
#authView{
  display:none;width:100%;height:100vh;
  background:var(--bg-page);
  align-items:center;justify-content:center;
}
#authView.active{display:flex}
.auth-card{
  background:var(--bg-surface);border:1px solid var(--border);
  border-radius:var(--radius-lg);padding:36px 32px;
  width:100%;max-width:380px;
  box-shadow:var(--shadow-md);
}
.auth-logo{display:flex;align-items:center;gap:8px;margin-bottom:28px}
.auth-logo-text{font-size:17px;font-weight:600;color:var(--blue-600)}
.auth-tabs{display:flex;gap:0;margin-bottom:22px;border-bottom:1px solid var(--border)}
.auth-tab{
  flex:1;padding:8px 0;font-size:13px;font-weight:500;font-family:inherit;
  background:none;border:none;border-bottom:2px solid transparent;
  cursor:pointer;color:var(--text-muted);transition:all 0.15s;margin-bottom:-1px;
}
.auth-tab.active{border-bottom-color:var(--blue-400);color:var(--blue-600)}
.auth-field{margin-bottom:14px}
.auth-field label{display:block;font-size:12px;font-weight:500;color:var(--text-secondary);margin-bottom:5px}
.auth-submit{
  width:100%;padding:9px;font-size:13px;font-weight:600;font-family:inherit;
  background:var(--blue-600);color:#fff;border:none;
  border-radius:var(--radius-sm);cursor:pointer;transition:background 0.15s;margin-top:4px;
}
.auth-submit:hover{background:var(--blue-800)}
[data-theme="dark"] .auth-submit{background:var(--blue-400)}
.auth-error{font-size:12px;color:#E24B4A;margin-top:10px;min-height:18px;text-align:center}
.auth-loading{font-size:12px;color:var(--text-muted);text-align:center;margin-top:10px}

/* user badge in topbar */
.user-badge{
  font-size:11px;color:var(--text-muted);
  display:flex;align-items:center;gap:5px;
}
.logout-btn{
  font-size:11px;padding:3px 9px;background:none;
  border:1px solid var(--border);border-radius:var(--radius-sm);
  cursor:pointer;color:var(--text-muted);transition:all 0.15s;font-family:inherit;
}
.logout-btn:hover{border-color:var(--border-hover);color:var(--text-primary)}

/* saving indicator */
.save-indicator{
  font-size:11px;color:var(--text-muted);
  opacity:0;transition:opacity 0.3s;
}
.save-indicator.show{opacity:1}
</style>
</head>
<body>

<!-- ══ AUTH VIEW ══ -->
<div id="authView">
  <div class="auth-card">
    <div class="auth-logo">
      <span class="ic" style="font-size:20px;color:var(--blue-400)"><svg viewBox="0 0 24 24"><rect x="3" y="3" width="7" height="7" rx="1"/><rect x="14" y="3" width="7" height="7" rx="1"/><rect x="3" y="14" width="7" height="7" rx="1"/><rect x="14" y="14" width="7" height="7" rx="1"/></svg></span>
      <span class="auth-logo-text">Daily Planner</span>
    </div>
    <div class="auth-tabs">
      <button class="auth-tab active" id="tabLogin">Sign in</button>
      <button class="auth-tab" id="tabSignup">Sign up</button>
    </div>
    <div id="authForm">
      <div class="auth-field">
        <label>Email</label>
        <input type="text" id="authEmail" placeholder="your@email.com" autocomplete="email">
      </div>
      <div class="auth-field">
        <label>Password</label>
        <input type="password" id="authPassword" placeholder="••••••••" autocomplete="current-password">
      </div>
      <button class="auth-submit" id="authSubmit">Sign in</button>
      <div class="auth-error" id="authError"></div>
    </div>
  </div>
</div>

<!-- ══ PLANNER VIEW ══ -->
<div id="plannerView" style="display:none">
<div class="app">

  <header class="topbar">
    <div class="topbar-logo"><span class="ic" style="font-size:18px;color:var(--blue-400)"><svg viewBox="0 0 24 24"><rect x="3" y="3" width="7" height="7" rx="1"/><rect x="14" y="3" width="7" height="7" rx="1"/><rect x="3" y="14" width="7" height="7" rx="1"/><rect x="14" y="14" width="7" height="7" rx="1"/></svg></span>Daily Planner</div>
    <div class="topbar-divider"></div>
    <span class="date-display-static" id="dateDisplayStatic"></span>
    <span class="today-pill">Today</span>
    <div class="topbar-right">
      <span class="save-indicator" id="saveIndicator">Saved ✓</span>
      <span class="user-badge" id="userBadge"></span>
      <button class="logout-btn" id="logoutBtn">Sign out</button>
      <div class="topbar-divider"></div>
      <button class="tb-btn" id="calBtn"><span class="ic"><svg viewBox="0 0 24 24"><rect x="4" y="5" width="16" height="16" rx="2"/><path d="M16 3v4M8 3v4M4 11h16"/></svg></span> Calendar</button>
      <div class="topbar-divider"></div>
      <button class="tb-btn" id="viewModeBtn"><span class="ic" id="viewModeIcon"><svg viewBox="0 0 24 24"><path d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z"/><circle cx="12" cy="12" r="3"/></svg></span> View</button>
      <button class="tb-btn" id="darkModeBtn"><span class="ic" id="darkModeIcon"><svg viewBox="0 0 24 24"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"/></svg></span></button>
      <div class="topbar-divider"></div>
      <button class="tb-btn" id="resetBtn"><span class="ic"><svg viewBox="0 0 24 24"><path d="M1 4v6h6"/><path d="M3.51 15a9 9 0 1 0 .49-3"/></svg></span> Reset</button>
    </div>
  </header>



  <!-- BLOCKS -->
  <div class="panel">
    <div class="panel-header">
      <span class="panel-title">Time Blocks</span>
    </div>
    <div class="panel-body" style="padding:14px 10px 14px 12px">
      <div class="time-label-row" id="timeLabels"></div>
      <div class="block-grid" id="blockGrid"></div>
    </div>
  </div>

  <!-- SCHEDULE -->
  <div class="panel">
    <div class="panel-header">
      <span class="panel-title">Schedule</span>
    </div>
    <div class="panel-body">
      <div id="memoRefArea"></div>
      <div id="scheduleHint" style="font-size:12px;color:var(--text-muted);display:flex;align-items:center;gap:6px;padding:0 2px 10px;border-bottom:1px solid var(--border);margin-bottom:10px">
        <span class="ic" style="font-size:14px;flex-shrink:0"><svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><line x1="12" y1="16" x2="12" y2="12"/><line x1="12" y1="8" x2="12.01" y2="8"/></svg></span>
        Drag across blocks to select a time range and add a schedule
      </div>
      <div class="schedule-list" id="scheduleList"></div>
    </div>
  </div>

  <!-- TODO -->
  <div class="panel" style="border-right:none">
    <div class="panel-header"><span class="panel-title">To-do</span></div>
    <div class="todo-input-row">
      <input type="text" id="todoInput" placeholder="Add a task...">
      <button class="primary-btn" id="addTodoBtn"><span class="ic"><svg viewBox="0 0 24 24"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg></span></button>
    </div>
    <div class="panel-body">
      <div class="todo-list" id="todoList"></div>
    </div>
  </div>

</div><!-- .app -->
</div><!-- #plannerView -->

<!-- SHORTCUT HELP OVERLAY -->
<div class="shortcut-overlay" id="shortcutOverlay">
  <div class="shortcut-box">
    <h3>Keyboard Shortcuts <button class="shortcut-close-btn" id="shortcutClose">✕</button></h3>

    <div class="sc-cat" id="sc-global">
      <button class="sc-cat-btn"><span>Global</span><span class="sc-arrow">▼</span></button>
      <div class="sc-cat-body">
        <div class="shortcut-row"><span>Time block grid</span><span><kbd>B</kbd></span></div>
        <div class="shortcut-row"><span>Focus todo</span><span><kbd>T</kbd></span></div>
        <div class="shortcut-row"><span>Focus schedule</span><span><kbd>S</kbd></span></div>
        <div class="shortcut-row"><span>Open calendar</span><span><kbd>C</kbd></span></div>
        <div class="shortcut-row"><span>Back to planner</span><span><kbd>P</kbd></span></div>
        <div class="shortcut-row"><span>View mode</span><span><kbd>V</kbd></span></div>
        <div class="shortcut-row"><span>Dark mode</span><span><kbd>D</kbd></span></div>
        <div class="shortcut-row"><span>Reset today</span><span><kbd>R</kbd></span></div>
        <div class="shortcut-row"><span>Close / cancel</span><span><kbd>Esc</kbd></span></div>
        <div class="shortcut-row"><span>This help</span><span><kbd>?</kbd></span></div>
      </div>
    </div>

    <div class="sc-cat" id="sc-blocks">
      <button class="sc-cat-btn"><span>Time Blocks</span><span class="sc-arrow">▼</span></button>
      <div class="sc-cat-body">
        <div class="shortcut-row"><span>Move focus</span><span><kbd>↑</kbd><kbd>↓</kbd><kbd>←</kbd><kbd>→</kbd></span></div>
        <div class="shortcut-row"><span>Select range</span><span><kbd>Shift</kbd>+<kbd>↑↓←→</kbd></span></div>
        <div class="shortcut-row"><span>Register schedule</span><span><kbd>Enter</kbd></span></div>
        <div class="shortcut-row"><span>Fill / erase</span><span><kbd>Space</kbd></span></div>
        <div class="shortcut-row"><span>Cancel selection</span><span><kbd>Esc</kbd></span></div>
      </div>
    </div>

    <div class="sc-cat" id="sc-schedule">
      <button class="sc-cat-btn"><span>Schedule</span><span class="sc-arrow">▼</span></button>
      <div class="sc-cat-body">
        <div class="shortcut-row"><span>Navigate</span><span><kbd>↑</kbd><kbd>↓</kbd></span></div>
        <div class="shortcut-row"><span>Edit event</span><span><kbd>Enter</kbd></span></div>
        <div class="shortcut-row"><span>Delete event</span><span><kbd>Del</kbd> / <kbd>⌫</kbd></span></div>
        <div class="shortcut-row"><span>Exit</span><span><kbd>Esc</kbd></span></div>
      </div>
    </div>

    <div class="sc-cat" id="sc-todo">
      <button class="sc-cat-btn"><span>To-do</span><span class="sc-arrow">▼</span></button>
      <div class="sc-cat-body">
        <div class="shortcut-row"><span>Focus list</span><span><kbd>↓</kbd> from input</span></div>
        <div class="shortcut-row"><span>Navigate</span><span><kbd>↑</kbd><kbd>↓</kbd></span></div>
        <div class="shortcut-row"><span>Delete item</span><span><kbd>Enter</kbd> or double-click</span></div>
      </div>
    </div>

    <div class="sc-cat" id="sc-calendar">
      <button class="sc-cat-btn"><span>Calendar</span><span class="sc-arrow">▼</span></button>
      <div class="sc-cat-body">
        <div class="shortcut-row"><span>Navigate dates</span><span><kbd>↑</kbd><kbd>↓</kbd><kbd>←</kbd><kbd>→</kbd></span></div>
        <div class="shortcut-row"><span>Open memo</span><span><kbd>Enter</kbd></span></div>
        <div class="shortcut-row"><span>Prev / next month</span><span><kbd>Shift</kbd>+<kbd>←</kbd><kbd>→</kbd></span></div>
        <div class="shortcut-row"><span>Clear focus</span><span><kbd>Esc</kbd></span></div>
      </div>
    </div>

  </div>
</div>

<!-- ── SCHEDULE REGISTER / EDIT POPUP ── -->
<div class="schedule-popup" id="schedulePopup">
  <div class="popup-time-range" id="popupTimeRange"></div>
  <div>
    <div class="field-label" style="margin-bottom:5px">Event name</div>
    <input type="text" id="popupTitle" placeholder="e.g. Team meeting, Lunch" autocomplete="off">
  </div>
  <div>
    <div class="field-label" style="margin-bottom:5px">Category</div>
    <div class="color-swatches" id="popupColorSwatches"></div>
  </div>
  <div style="display:flex;gap:7px;margin-top:2px">
    <button class="primary-btn" id="popupConfirmBtn" style="flex:1;justify-content:center"></button>
    <button id="popupCancelBtn" style="flex:1;height:33px;font-size:12px;font-weight:500;font-family:inherit;background:var(--bg-surface);border:1px solid var(--border);border-radius:var(--radius-sm);cursor:pointer;color:var(--text-secondary);transition:all 0.15s">Cancel</button>
  </div>
</div>

<!-- ══ CALENDAR VIEW ══ -->
<div id="calendarView">
  <header class="cal-topbar">
    <button class="cal-back-btn" id="calBackBtn"><span class="ic"><svg viewBox="0 0 24 24"><line x1="19" y1="12" x2="5" y2="12"/><polyline points="12 19 5 12 12 5"/></svg></span> Planner</button>
    <span class="cal-title">Calendar</span>
    <div class="cal-month-nav">
      <button class="cal-month-btn" id="calPrevMonth"><span class="ic" style="font-size:15px"><svg viewBox="0 0 24 24"><polyline points="15 18 9 12 15 6"/></svg></span></button>
      <span class="cal-month-label" id="calMonthLabel"></span>
      <button class="cal-month-btn" id="calNextMonth"><span class="ic" style="font-size:15px"><svg viewBox="0 0 24 24"><polyline points="9 18 15 12 9 6"/></svg></span></button>
    </div>
    <button class="tb-btn" id="calDarkBtn" style="margin-left:10px"><span class="ic" id="calDarkIcon"><svg viewBox="0 0 24 24"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"/></svg></span></button>
  </header>
  <div class="cal-body">
    <div class="cal-grid-wrap">
      <div class="cal-day-headers" id="calDayHeaders"></div>
      <div class="cal-grid" id="calGrid"></div>
    </div>
  </div>
</div>

<!-- RESET MODAL -->
<div class="modal-overlay" id="resetModal">
  <div class="modal">
    <div class="modal-title">Reset Confirmation</div>
    <div class="modal-desc">Today's schedule and time blocks will be cleared. This can't be undone.</div>
    <div class="modal-actions">
      <button class="modal-cancel" id="resetCancel">Cancel</button>
      <button class="modal-confirm" id="resetConfirm">Reset</button>
    </div>
  </div>
</div>

<!-- MEMO MODAL -->
<div class="modal-overlay" id="memoModal">
  <div class="memo-modal">
    <div class="memo-modal-date" id="memoModalDate"></div>
    <div class="memo-modal-title">Notes</div>
    <div class="memo-modal-list" id="memoModalList"></div>
    <div class="memo-modal-add">
      <input type="text" id="memoModalInput" placeholder="Add a note...">
      <button class="primary-btn" id="memoModalAddBtn"><span class="ic"><svg viewBox="0 0 24 24" style="width:13px;height:13px;stroke:currentColor;fill:none;stroke-width:2;stroke-linecap:round"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg></span></button>
    </div>
    <div class="modal-actions" style="margin-top:14px">
      <button class="modal-cancel" id="memoModalClose">Close</button>
    </div>
  </div>
</div>

<script type="module">
import { createClient } from 'https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2/+esm';
// ══════════════════════════════════════
//  SUPABASE
// ══════════════════════════════════════
const SUPABASE_URL = 'https://aortzwmwoqabvdxsivsv.supabase.co';
const SUPABASE_KEY = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImFvcnR6d213b3FhYnZkeHNpdnN2Iiwicm9sZSI6ImFub24iLCJpYXQiOjE3ODAzMDM0MTQsImV4cCI6MjA5NTg3OTQxNH0.XuU2UsYaGZVE9PqT2xC2fi3mJ1jh3gb7_cNpaPzzSKk';
const sb = createClient(SUPABASE_URL, SUPABASE_KEY);

let currentUser = null;
let remoteData = { blocks:{}, schedules:{}, notes:{}, todos:[] };
let saveTimer = null;

// ── load all data from Supabase ──
async function loadRemoteData(){
  if(!currentUser) return;
  try {
    const timeout = new Promise((_, reject) =>
      setTimeout(() => reject(new Error('timeout')), 3000)
    );
    const fetchData = sb.from('user_data').select('*').eq('id', currentUser.id).single();
    const { data, error } = await Promise.race([fetchData, timeout]);
    if(error){
      remoteData = { blocks:{}, schedules:{}, notes:{}, todos:[] };
      return;
    }
    if(!data){ remoteData = { blocks:{}, schedules:{}, notes:{}, todos:[] }; return; }
    remoteData = {
      blocks:    (data.blocks    && typeof data.blocks    === 'object') ? data.blocks    : {},
      schedules: (data.schedules && typeof data.schedules === 'object') ? data.schedules : {},
      notes:     (data.notes     && typeof data.notes     === 'object') ? data.notes     : {},
      todos:     Array.isArray(data.todos) ? data.todos : []
    };
  } catch(e) {
    remoteData = { blocks:{}, schedules:{}, notes:{}, todos:[] };
  }
}

// ── save all data to Supabase (debounced 800ms) ──
function scheduleSave(){
  clearTimeout(saveTimer);
  saveTimer = setTimeout(async ()=>{
    if(!currentUser) return;
    const payload = {
      id:         currentUser.id,
      blocks:     remoteData.blocks    || {},
      schedules:  remoteData.schedules || {},
      notes:      remoteData.notes     || {},
      todos:      remoteData.todos     || [],
      updated_at: new Date().toISOString()
    };
    const { error } = await sb.from('user_data').upsert(payload, { onConflict: 'id' });
    if(!error){
      const ind = document.getElementById('saveIndicator');
      if(ind){ ind.classList.add('show'); setTimeout(()=>ind.classList.remove('show'), 1800); }
    } else {
      console.error('save error', error);
    }
  }, 800);
}

// ══════════════════════════════════════
//  CONSTANTS & STORAGE
// ══════════════════════════════════════
const MONTHS_SHORT=['Jan','Feb','Mar','Apr','May','Jun','Jul','Aug','Sep','Oct','Nov','Dec'];
const PALETTE = ['#E24B4A','#D85A30','#EF9F27','#639922','#1D9E75','#378ADD','#7F77DD','#D4537E','#888780'];
const PALETTE_EMOJI = ['🚨','🍽️','🤝','🌿','✍️','📖','🎮','👀','➡️'];
const PALETTE_LABEL = ['Important','Meals / Chores','Appointment','Rest','Creative','Study','Entertainment','Self-care','Etc.'];
const START_HOUR=5, END_HOUR=24, COLS=6, BLOCK_MIN=10;
const TOTAL_BLOCKS=(END_HOUR-START_HOUR)*COLS;
const TOTAL_ROWS=END_HOUR-START_HOUR;

const get  = k=>{ try{return JSON.parse(localStorage.getItem(k)||'null')}catch{return null} };
const set  = (k,v)=>localStorage.setItem(k,JSON.stringify(v));

// remote-aware data accessors
const getBlocks    = dk=>(remoteData.blocks[dk]   || {});
const saveBlocks   = (dk,d)=>{ remoteData.blocks[dk]=d;    scheduleSave(); };
const getSchedules = dk=>(remoteData.schedules[dk]|| []);
const saveSchedules= (dk,d)=>{ remoteData.schedules[dk]=d; scheduleSave(); };
const getNotes     = dk=>(remoteData.notes[dk]    || []);
const saveNotes    = (dk,d)=>{ remoteData.notes[dk]=d;     scheduleSave(); };
const getTodos     = ()=>(remoteData.todos         || []);
const saveTodos    = d=>{ remoteData.todos=d;               scheduleSave(); };
const getSelColor  = ()=>get('bp_color')??0;
const saveSelColor = i=>set('bp_color',i);

// ══════════════════════════════════════
//  DATE HELPERS (today only in planner)
// ══════════════════════════════════════
function pad(n){return String(n).padStart(2,'0')}
function todayKey(){
  const d=new Date();
  return `${d.getFullYear()}-${pad(d.getMonth()+1)}-${pad(d.getDate())}`;
}
function formatDate(key){
  const [y,m,d]=key.split('-').map(Number);
  const days=['Sun','Mon','Tue','Wed','Thu','Fri','Sat'];
  const dt=new Date(y,m-1,d);
  return `${days[dt.getDay()]}, ${MONTHS_SHORT[m-1]} ${d}`;
}
function blockToTime(idx){
  const tot=START_HOUR*60+idx*BLOCK_MIN;
  return `${pad(Math.floor(tot/60)%24)}:${pad(tot%60)}`;
}
function timeToBlock(hhmm){
  const [h,m]=hhmm.split(':').map(Number);
  return Math.floor((h*60+m-START_HOUR*60)/BLOCK_MIN);
}
function esc(s){return String(s).replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/\x22/g,'&quot;')}

// ══════════════════════════════════════
//  THEME
// ══════════════════════════════════════
function isDark(){return document.documentElement.getAttribute('data-theme')==='dark'}
function applyTheme(dark){
  document.documentElement.setAttribute('data-theme',dark?'dark':'');
  set('bp_dark',dark);
  const ico=dark?SVG_SUN:SVG_MOON;
  document.getElementById('darkModeBtn').innerHTML=ico;
  document.getElementById('calDarkBtn').innerHTML=ico;
}
document.getElementById('darkModeBtn').addEventListener('click',()=>applyTheme(!isDark()));
document.getElementById('calDarkBtn').addEventListener('click',()=>applyTheme(!isDark()));

// ══════════════════════════════════════
//  VIEW MODE
// ══════════════════════════════════════
const SVG_EYE    = '<span class="ic"><svg viewBox="0 0 24 24" style="width:14px;height:14px;stroke:currentColor;fill:none;stroke-width:1.5;stroke-linecap:round;stroke-linejoin:round"><path d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z"/><circle cx="12" cy="12" r="3"/></svg></span>';
const SVG_EYE_OFF= '<span class="ic"><svg viewBox="0 0 24 24" style="width:14px;height:14px;stroke:currentColor;fill:none;stroke-width:1.5;stroke-linecap:round;stroke-linejoin:round"><path d="M17.94 17.94A10.07 10.07 0 0 1 12 20c-7 0-11-8-11-8a18.45 18.45 0 0 1 5.06-5.94M9.9 4.24A9.12 9.12 0 0 1 12 4c7 0 11 8 11 8a18.5 18.5 0 0 1-2.16 3.19m-6.72-1.07a3 3 0 1 1-4.24-4.24"/><line x1="1" y1="1" x2="23" y2="23"/></svg></span>';
const SVG_MOON   = '<span class="ic"><svg viewBox="0 0 24 24" style="width:14px;height:14px;stroke:currentColor;fill:none;stroke-width:1.5;stroke-linecap:round;stroke-linejoin:round"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"/></svg></span>';
const SVG_SUN    = '<span class="ic"><svg viewBox="0 0 24 24" style="width:14px;height:14px;stroke:currentColor;fill:none;stroke-width:1.5;stroke-linecap:round;stroke-linejoin:round"><circle cx="12" cy="12" r="5"/><line x1="12" y1="1" x2="12" y2="3"/><line x1="12" y1="21" x2="12" y2="23"/><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"/><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"/><line x1="1" y1="12" x2="3" y2="12"/><line x1="21" y1="12" x2="23" y2="12"/><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"/><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"/></svg></span>';
const SVG_CLOCK  = '<span class="ic"><svg viewBox="0 0 24 24" style="width:11px;height:11px;stroke:currentColor;fill:none;stroke-width:1.5;stroke-linecap:round;stroke-linejoin:round"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg></span>';
const SVG_TRASH  = '<span class="ic"><svg viewBox="0 0 24 24" style="width:14px;height:14px;stroke:currentColor;fill:none;stroke-width:1.5;stroke-linecap:round;stroke-linejoin:round"><polyline points="3 6 5 6 21 6"/><path d="M19 6l-1 14H6L5 6"/><path d="M10 11v6M14 11v6"/><path d="M9 6V4h6v2"/></svg></span>';
const SVG_CHECK  = '<span class="ic"><svg viewBox="0 0 24 24" style="width:17px;height:17px;stroke:currentColor;fill:none;stroke-width:1.5;stroke-linecap:round;stroke-linejoin:round"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg></span>';
const SVG_PIN    = '<span class="ic"><svg viewBox="0 0 24 24" style="width:13px;height:13px;stroke:currentColor;fill:none;stroke-width:1.5;stroke-linecap:round;stroke-linejoin:round"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"/><circle cx="12" cy="10" r="3"/></svg></span>';
const SVG_X      = '<span class="ic"><svg viewBox="0 0 24 24" style="width:12px;height:12px;stroke:currentColor;fill:none;stroke-width:2;stroke-linecap:round"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg></span>';
const SVG_PLUS   = '<span class="ic"><svg viewBox="0 0 24 24" style="width:13px;height:13px;stroke:currentColor;fill:none;stroke-width:2;stroke-linecap:round"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg></span>';

let viewMode=false;
function toggleViewMode(){
  viewMode=!viewMode;
  document.body.classList.toggle('view-mode',viewMode);
  const btn=document.getElementById('viewModeBtn');
  btn.classList.toggle('active',viewMode);
  btn.innerHTML=viewMode?SVG_EYE_OFF+' Edit':SVG_EYE+' View';
}
document.getElementById('viewModeBtn').addEventListener('click',toggleViewMode);

// ══════════════════════════════════════
//  BLOCK GRID  — drag-to-select & erase
// ══════════════════════════════════════
// drag state
let dragState=null;
// dragState = { mode: 'select'|'erase', startIdx, endIdx }

function buildScMap(dk){
  const map={};
  getSchedules(dk).forEach(s=>{
    const si=timeToBlock(s.start),ei=timeToBlock(s.end);
    for(let i=si;i<ei&&i<TOTAL_BLOCKS;i++) if(i>=0) map[i]={color:s.color,title:s.title};
  });
  return map;
}

function renderTimeLabels(){
  const el=document.getElementById('timeLabels');
  el.innerHTML='<div></div>';
  for(let c=0;c<COLS;c++)
    el.innerHTML+=`<div class="time-col-label">:${pad(c*10)}</div>`;
}

function renderBlocks(){
  const dk=todayKey();
  const blocks=getBlocks(dk);
  const scMap=buildScMap(dk);
  const grid=document.getElementById('blockGrid');
  grid.innerHTML='';

  const now=new Date();
  const nowIdx=timeToBlock(`${pad(now.getHours())}:${pad(now.getMinutes())}`);

  for(let row=0;row<TOTAL_ROWS;row++){
    const rowEl=document.createElement('div');
    rowEl.className='block-row';
    const lbl=document.createElement('div');
    lbl.className='row-hour-label';
    lbl.textContent=((START_HOUR+row)%24)+':00';
    rowEl.appendChild(lbl);

    for(let col=0;col<COLS;col++){
      const idx=row*COLS+col;
      const isSched=!!scMap[idx];
      const isNow=idx===nowIdx;
      const color=isSched?scMap[idx].color:blocks[idx];
      const b=document.createElement('div');
      b.className='block'+(color?' filled':'')+(isSched?' schedule-block':'')+(isNow?' now-block':'');
      if(color) b.style.background=color;
      b.dataset.idx=idx;
      b.dataset.sched=isSched?'1':'0';
      rowEl.appendChild(b);
    }
    grid.appendChild(rowEl);
  }
}

// ── drag logic ──
function getBlockEl(idx){return document.querySelector(`.block[data-idx="${idx}"]`)}

function applyDragPreview(startIdx,endIdx){
  // clear all previews
  document.querySelectorAll('.block.drag-preview').forEach(b=>b.classList.remove('drag-preview'));
  const lo=Math.min(startIdx,endIdx), hi=Math.max(startIdx,endIdx);
  for(let i=lo;i<=hi;i++){
    const el=getBlockEl(i);
    if(el&&el.dataset.sched==='0') el.classList.add('drag-preview');
  }
}
function clearDragPreview(){
  document.querySelectorAll('.block.drag-preview').forEach(b=>b.classList.remove('drag-preview'));
}

const blockGrid=document.getElementById('blockGrid');

blockGrid.addEventListener('mousedown',e=>{
  if(viewMode) return;
  const b=e.target.closest('.block');
  if(!b) return;
  const idx=+b.dataset.idx;
  const isSched=b.dataset.sched==='1';
  const isFilled=b.classList.contains('filled');

  if(isSched) return; // can't drag on schedule blocks

  if(isFilled){
    // erase mode: single click erases, drag erases range
    dragState={mode:'erase',startIdx:idx,endIdx:idx};
    eraseBlock(idx);
  } else {
    // select mode for schedule registration
    dragState={mode:'select',startIdx:idx,endIdx:idx};
    applyDragPreview(idx,idx);
  }
  e.preventDefault();
});

blockGrid.addEventListener('mouseover',e=>{
  if(!dragState||viewMode) return;
  const b=e.target.closest('.block');
  if(!b) return;
  const idx=+b.dataset.idx;
  dragState.endIdx=idx;

  if(dragState.mode==='erase'){
    // erase all in range
    const lo=Math.min(dragState.startIdx,idx), hi=Math.max(dragState.startIdx,idx);
    for(let i=lo;i<=hi;i++) eraseBlock(i);
  } else {
    applyDragPreview(dragState.startIdx,idx);
  }
});

document.addEventListener('mouseup',e=>{
  if(!dragState||viewMode){ dragState=null; return; }
  if(dragState.mode==='select'){
    clearDragPreview();
    const lo=Math.min(dragState.startIdx,dragState.endIdx);
    const hi=Math.max(dragState.startIdx,dragState.endIdx);
    // check if any non-schedule blocks selected
    let hasEmpty=false;
    for(let i=lo;i<=hi;i++){
      const el=getBlockEl(i);
      if(el&&el.dataset.sched==='0'&&!el.classList.contains('filled')) hasEmpty=true;
    }
    if(hasEmpty) openSchedulePopup(lo,hi,e);
    else if(lo===hi){
      // single filled block: toggle off
      eraseBlock(lo);
    }
  }
  dragState=null;
});

function eraseBlock(idx){
  const el=getBlockEl(idx);
  if(!el||el.dataset.sched==='1') return;
  const dk=todayKey();
  const blocks=getBlocks(dk);
  delete blocks[idx];
  saveBlocks(dk,blocks);
  el.classList.remove('filled','drag-preview');
  el.style.background='';
}

// ══════════════════════════════════════
//  SCHEDULE POPUP  (create + edit)
// ══════════════════════════════════════
let popupRange={lo:0,hi:0};
let popupEditIdx=-1; // -1 = create mode, >=0 = edit mode (index into schedules)

const SVG_ADD='<span class="ic"><svg viewBox="0 0 24 24" style="width:13px;height:13px;stroke:currentColor;fill:none;stroke-width:2;stroke-linecap:round;stroke-linejoin:round"><polyline points="20 6 9 17 4 12"/></svg></span>';
const SVG_SAVE='<span class="ic"><svg viewBox="0 0 24 24" style="width:13px;height:13px;stroke:currentColor;fill:none;stroke-width:2;stroke-linecap:round;stroke-linejoin:round"><path d="M19 21H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11l5 5v11a2 2 0 0 1-2 2z"/><polyline points="17 21 17 13 7 13 7 21"/><polyline points="7 3 7 8 15 8"/></svg></span>';

function openSchedulePopup(lo, hi, mouseEvent, editIdx=-1){
  popupRange={lo,hi};
  popupEditIdx=editIdx;

  if(editIdx>=0){
    // edit mode — pre-fill from existing schedule
    const s=getSchedules(todayKey())[editIdx];
    document.getElementById('popupTimeRange').textContent=`${s.start} – ${s.end}`;
    document.getElementById('popupTitle').value=s.title;
    const ci=PALETTE.indexOf(s.color); saveSelColor(ci>=0?ci:0);
    document.getElementById('popupConfirmBtn').innerHTML=SVG_SAVE+' Save';
  } else {
    document.getElementById('popupTimeRange').textContent=`${blockToTime(lo)} – ${blockToTime(hi+1)}`;
    document.getElementById('popupTitle').value='';
    document.getElementById('popupConfirmBtn').innerHTML=SVG_ADD+' Add';
  }
  renderPopupColors();

  const popup=document.getElementById('schedulePopup');
  popup.classList.add('open');

  // position near mouse, keep inside viewport
  const pw=330, ph=310;
  let x=mouseEvent.clientX+14, y=mouseEvent.clientY-ph/2;
  if(x+pw>window.innerWidth-8) x=mouseEvent.clientX-pw-14;
  if(y<8) y=8;
  if(y+ph>window.innerHeight-8) y=window.innerHeight-ph-8;
  popup.style.left=x+'px';
  popup.style.top=y+'px';

  setTimeout(()=>document.getElementById('popupTitle').focus(),50);
}

function renderPopupColors(){
  const c=document.getElementById('popupColorSwatches');
  c.innerHTML='';
  const sel=getSelColor();
  PALETTE.forEach((col,i)=>{
    const btn=document.createElement('button');
    btn.className='color-btn'+(i===sel?' active':'');
    // active border color matches the palette color
    if(i===sel) btn.style.borderColor=col;
    btn.style.color=col; // used for currentColor border on active
    btn.tabIndex=0;
    btn.innerHTML=`<span class="cb-dot" style="background:${col}"></span><span class="cb-label">${PALETTE_EMOJI[i]} ${PALETTE_LABEL[i]}</span>`;
    btn.addEventListener('click',()=>{ saveSelColor(i); renderPopupColors(); });
    c.appendChild(btn);
  });
}

function closeSchedulePopup(restoreSchedFocus=false){
  document.getElementById('schedulePopup').classList.remove('open');
  clearDragPreview();
  if(restoreSchedFocus){
    setTimeout(()=>{
      document.getElementById('scheduleList').focus();
      renderSchedulesFocused();
    }, 0);
  }
}

function confirmSchedule(){
  const title=document.getElementById('popupTitle').value.trim();
  if(!title){ document.getElementById('popupTitle').focus(); showToast('Please enter an event name'); return; }

  const dk=todayKey();
  const color=PALETTE[getSelColor()];
  const all=getSchedules(dk);
  const wasEdit=popupEditIdx>=0;

  if(wasEdit){
    const old=all[popupEditIdx];
    const blocks=getBlocks(dk);
    const si=timeToBlock(old.start), ei=timeToBlock(old.end);
    for(let i=si;i<ei&&i<TOTAL_BLOCKS;i++) if(i>=0) blocks[i]=color;
    saveBlocks(dk,blocks);
    all[popupEditIdx]={...old, title, color};
    saveSchedules(dk,all);
  } else {
    all.push({title, start:blockToTime(popupRange.lo), end:blockToTime(popupRange.hi+1), color});
    saveSchedules(dk,all);
    const blocks=getBlocks(dk);
    for(let i=popupRange.lo;i<=popupRange.hi;i++) blocks[i]=color;
    saveBlocks(dk,blocks);
  }

  closeSchedulePopup(wasEdit);
  renderBlocks();
  renderSchedules();
}

document.getElementById('popupConfirmBtn').addEventListener('click',confirmSchedule);
document.getElementById('popupCancelBtn').addEventListener('click',()=>closeSchedulePopup(popupEditIdx>=0));

document.getElementById('popupTitle').addEventListener('keydown',e=>{
  if(e.key==='Enter'){ e.preventDefault(); confirmSchedule(); }
  if(e.key==='Escape'){ e.preventDefault(); closeSchedulePopup(popupEditIdx>=0); }
  // ArrowDown from title → move to color swatches
  if(e.key==='ArrowDown'){
    e.preventDefault();
    const swatches=document.querySelectorAll('#popupColorSwatches .color-btn');
    swatches[getSelColor()]?.focus();
  }
});

// color swatch keyboard nav (2-col grid)
document.getElementById('popupColorSwatches').addEventListener('keydown',e=>{
  const swatches=[...document.querySelectorAll('#popupColorSwatches .color-btn')];
  const cur=swatches.indexOf(document.activeElement);
  if(e.key==='ArrowRight'){
    e.preventDefault();
    const next=cur+1;
    if(next<swatches.length){ saveSelColor(next); renderPopupColors(); document.querySelectorAll('#popupColorSwatches .color-btn')[next]?.focus(); }
  } else if(e.key==='ArrowLeft'){
    e.preventDefault();
    const prev=cur-1;
    if(prev>=0){ saveSelColor(prev); renderPopupColors(); document.querySelectorAll('#popupColorSwatches .color-btn')[prev]?.focus(); }
  } else if(e.key==='ArrowDown'){
    e.preventDefault();
    const next=cur+2;
    if(next<swatches.length){ saveSelColor(next); renderPopupColors(); document.querySelectorAll('#popupColorSwatches .color-btn')[next]?.focus(); }
    else document.getElementById('popupConfirmBtn').focus();
  } else if(e.key==='ArrowUp'){
    e.preventDefault();
    const prev=cur-2;
    if(prev>=0){ saveSelColor(prev); renderPopupColors(); document.querySelectorAll('#popupColorSwatches .color-btn')[prev]?.focus(); }
    else document.getElementById('popupTitle').focus();
  } else if(e.key==='Enter'||e.key===' '){
    e.preventDefault(); confirmSchedule();
  } else if(e.key==='Escape'){
    e.preventDefault(); closeSchedulePopup(popupEditIdx>=0);
  } else if(e.key==='Tab'){
    e.preventDefault();
    if(e.shiftKey) document.getElementById('popupTitle').focus();
    else document.getElementById('popupConfirmBtn').focus();
  }
});

// confirm/cancel button keyboard
document.getElementById('popupConfirmBtn').addEventListener('keydown',e=>{
  if(e.key==='Escape'){ e.preventDefault(); closeSchedulePopup(popupEditIdx>=0); }
  if(e.key==='ArrowUp'){
    e.preventDefault();
    const swatches=document.querySelectorAll('#popupColorSwatches .color-btn');
    swatches[getSelColor()]?.focus();
  }
  if(e.key==='Tab'&&e.shiftKey){
    e.preventDefault();
    const swatches=document.querySelectorAll('#popupColorSwatches .color-btn');
    swatches[getSelColor()]?.focus();
  }
});
document.getElementById('popupCancelBtn').addEventListener('keydown',e=>{
  if(e.key==='Escape'){ e.preventDefault(); closeSchedulePopup(popupEditIdx>=0); }
});

// close popup on outside click
document.addEventListener('mousedown',e=>{
  const popup=document.getElementById('schedulePopup');
  if(popup.classList.contains('open')&&!popup.contains(e.target)&&!e.target.closest('.block')){
    closeSchedulePopup();
  }
});

// ══════════════════════════════════════
//  SCHEDULE LIST
// ══════════════════════════════════════
function renderSchedules(){
  // memo ref
  const dk=todayKey();
  const memoRef=document.getElementById('memoRefArea');
  memoRef.innerHTML='';
  const notes=getNotes(dk);
  if(notes.length){
    const banner=document.createElement('div');
    banner.className='memo-ref-banner';
    let html=`<div class="memo-ref-title">📌 Today's Notes</div>`;
    notes.forEach(n=>{ html+=`<div class="memo-ref-item"><span style="width:5px;height:5px;border-radius:50%;background:currentColor;display:inline-block;opacity:0.5;flex-shrink:0"></span>${esc(n)}</div>`; });
    banner.innerHTML=html;
    memoRef.appendChild(banner);
  }

  const list=document.getElementById('scheduleList');
  const allScheds=getSchedules(dk);
  // sort by time but keep track of original indices
  const scheds=allScheds.map((s,i)=>({...s,_origIdx:i})).sort((a,b)=>a.start.localeCompare(b.start));
  list.innerHTML='';
  if(!scheds.length){
    list.innerHTML='<div class="empty-hint">Drag blocks to add a schedule</div>';
    return;
  }
  const lbl=document.createElement('div'); lbl.className='section-lbl'; lbl.textContent='Events';
  list.appendChild(lbl);
  scheds.forEach((s,i)=>{
    const item=document.createElement('div');
    item.className='schedule-item';
    item.dataset.origIdx=s._origIdx;
    item.innerHTML=`
      <div class="schedule-bookmark" style="background:${s.color}"></div>
      <div class="schedule-content">
        <div class="schedule-title">${PALETTE_EMOJI[PALETTE.indexOf(s.color)]||''} ${esc(s.title)}</div>
        <div class="schedule-time-tag">${SVG_CLOCK}${s.start} – ${s.end}</div>
      </div>
      <button class="schedule-del" data-orig-idx="${s._origIdx}" title="Delete" style="pointer-events:auto">${SVG_TRASH}</button>
    `;
    list.appendChild(item);
  });
  list.querySelectorAll('.schedule-del').forEach(btn=>{
    btn.addEventListener('click',()=>{
      if(viewMode) return;
      const dk=todayKey();
      const all=getSchedules(dk);
      const origIdx=+btn.dataset.origIdx;
      const removed=all[origIdx];
      if(removed){
        const blocks=getBlocks(dk);
        const si=timeToBlock(removed.start), ei=timeToBlock(removed.end);
        for(let i=si;i<ei&&i<TOTAL_BLOCKS;i++) if(i>=0) delete blocks[i];
        saveBlocks(dk,blocks);
      }
      all.splice(origIdx,1);
      saveSchedules(dk,all);
      renderSchedules(); renderBlocks();
    });
  });
}

// ══════════════════════════════════════
//  TODO
// ══════════════════════════════════════
let todoFocusIdx = -1;

function renderTodos(){
  const todos=getTodos();
  const list=document.getElementById('todoList');
  list.innerHTML='';
  if(!todos.length){ list.innerHTML='<div class="empty-hint">Add things to do today</div>'; todoFocusIdx=-1; return; }
  todos.forEach((t,i)=>{
    const item=document.createElement('div');
    item.className='todo-item'+(i===todoFocusIdx?' kb-focus':'');
    item.tabIndex=0;
    item.dataset.idx=i;
    item.innerHTML=`${SVG_CHECK.replace('class="ic"','class="ic todo-check"')}<span class="todo-text">${esc(t)}</span>`;
    // double-click to delete
    item.addEventListener('dblclick',()=>{ if(viewMode) return; deleteTodo(i); });
    // single click = focus
    item.addEventListener('click',()=>{
      if(viewMode) return;
      todoFocusIdx=i;
      renderTodos();
      document.querySelectorAll('.todo-item')[i]?.focus();
    });
    // keyboard on item
    item.addEventListener('keydown',e=>{
      if(viewMode) return;
      if(e.key==='Enter'||e.key===' '){ e.preventDefault(); deleteTodo(i); }
      if(e.key==='ArrowDown'){ e.preventDefault(); moveTodoFocus(1); }
      if(e.key==='ArrowUp'){ e.preventDefault(); moveTodoFocus(-1); }
      if(e.key==='Escape'){ todoFocusIdx=-1; renderTodos(); document.getElementById('todoInput').focus(); }
    });
    list.appendChild(item);
  });
}

function deleteTodo(i){
  const arr=getTodos(); arr.splice(i,1); saveTodos(arr);
  todoFocusIdx=Math.min(i, arr.length-1);
  renderTodos();
  if(arr.length>0) document.querySelectorAll('.todo-item')[todoFocusIdx]?.focus();
}

function moveTodoFocus(dir){
  const todos=getTodos();
  if(!todos.length) return;
  todoFocusIdx=Math.max(0,Math.min(todos.length-1,(todoFocusIdx<0?0:todoFocusIdx)+dir));
  renderTodos();
  document.querySelectorAll('.todo-item')[todoFocusIdx]?.focus();
}

function addTodo(){
  if(viewMode) return;
  const val=document.getElementById('todoInput').value.trim();
  if(!val) return;
  const todos=getTodos(); todos.push(val); saveTodos(todos);
  document.getElementById('todoInput').value=''; todoFocusIdx=-1; renderTodos();
}
document.getElementById('addTodoBtn').addEventListener('click',addTodo);
document.getElementById('todoInput').addEventListener('keydown',e=>{
  if(e.key==='Enter') addTodo();
  if(e.key==='ArrowDown'){ e.preventDefault(); moveTodoFocus(todoFocusIdx<0?0:1); }
});

// ══════════════════════════════════════
//  RESET
// ══════════════════════════════════════
document.getElementById('resetBtn').addEventListener('click',()=>{ document.getElementById('resetModal').classList.add('open'); });
document.getElementById('resetCancel').addEventListener('click',()=>{ document.getElementById('resetModal').classList.remove('open'); });
document.getElementById('resetConfirm').addEventListener('click',()=>{
  const dk=todayKey(); saveBlocks(dk,{}); saveSchedules(dk,[]);
  document.getElementById('resetModal').classList.remove('open');
  renderBlocks(); renderSchedules();
});
document.getElementById('resetModal').addEventListener('click',e=>{ if(e.target===e.currentTarget) e.currentTarget.classList.remove('open'); });

// ══════════════════════════════════════
//  CALENDAR VIEW
// ══════════════════════════════════════
let calYear,calMonth;

let calFocusDk = ''; // currently focused date key in calendar

function calCells(){
  // returns only non-empty, non-past cells with their dk
  return [...document.querySelectorAll('#calGrid .cal-cell:not(.cal-cell-empty)')];
}

function getCalCellByDk(dk){
  return [...document.querySelectorAll('#calGrid .cal-cell:not(.cal-cell-empty)')]
    .find(el=>el.dataset.dk===dk);
}

function setCalFocus(dk){
  calFocusDk=dk;
  document.querySelectorAll('#calGrid .cal-cell').forEach(el=>{
    el.classList.toggle('kb-focus', el.dataset.dk===dk);
  });
  getCalCellByDk(dk)?.scrollIntoView({block:'nearest',behavior:'smooth'});
}

function clearCalFocus(){
  calFocusDk='';
  document.querySelectorAll('#calGrid .cal-cell.kb-focus').forEach(el=>el.classList.remove('kb-focus'));
}

// attach dk to each cell in renderCalendar
function openCalendar(){
  const now=new Date(); calYear=now.getFullYear(); calMonth=now.getMonth();
  document.getElementById('plannerView').classList.add('hidden');
  document.getElementById('calendarView').classList.add('active');
  renderCalendar();
  // focus today after render
  setTimeout(()=>{
    calFocusDk=todayKey();
    setCalFocus(calFocusDk);
    document.getElementById('calGrid').focus();
  }, 50);
}
function closeCalendar(){
  clearCalFocus();
  document.getElementById('calendarView').classList.remove('active');
  document.getElementById('plannerView').classList.remove('hidden');
  renderSchedules();
}

// calendar grid keyboard handler
document.getElementById('calGrid').setAttribute('tabindex','0');
document.getElementById('calGrid').addEventListener('keydown',e=>{
  if(!calFocusDk) return;

  const [cy,cm,cd]=calFocusDk.split('-').map(Number);
  const cur=new Date(cy,cm-1,cd);
  let next=null;

  if(e.key==='ArrowRight'){ e.preventDefault(); next=new Date(cur); next.setDate(cur.getDate()+1); }
  else if(e.key==='ArrowLeft'){ e.preventDefault(); next=new Date(cur); next.setDate(cur.getDate()-1); }
  else if(e.key==='ArrowDown'){ e.preventDefault(); next=new Date(cur); next.setDate(cur.getDate()+7); }
  else if(e.key==='ArrowUp'){ e.preventDefault(); next=new Date(cur); next.setDate(cur.getDate()-7); }
  else if(e.key==='Enter'){
    e.preventDefault();
    const isPast=cur<new Date(new Date().toDateString());
    if(!isPast) openMemoModal(calFocusDk);
    return;
  }
  else if(e.key==='Escape'){
    e.preventDefault(); clearCalFocus(); return;
  }

  if(next){
    const dk=`${next.getFullYear()}-${pad(next.getMonth()+1)}-${pad(next.getDate())}`;
    // if moved to a different month, navigate there first
    if(next.getMonth()!==cm-1||next.getFullYear()!==cy){
      calYear=next.getFullYear(); calMonth=next.getMonth();
      renderCalendar();
    }
    setCalFocus(dk);
  }
});

// Shift+←→ = prev/next month (works regardless of cell focus)
document.getElementById('calendarView').addEventListener('keydown',e=>{
  if(e.key==='ArrowLeft'&&e.shiftKey){ e.preventDefault(); calMonth--; if(calMonth<0){calMonth=11;calYear--;} renderCalendar(); }
  else if(e.key==='ArrowRight'&&e.shiftKey){ e.preventDefault(); calMonth++; if(calMonth>11){calMonth=0;calYear++;} renderCalendar(); }
});

// memo modal: Esc → close and restore calendar focus
document.getElementById('memoModalClose').addEventListener('click',()=>{
  document.getElementById('memoModal').classList.remove('open');
  if(calFocusDk) setTimeout(()=>document.getElementById('calGrid').focus(), 50);
});
document.getElementById('memoModal').addEventListener('click',e=>{
  if(e.target===e.currentTarget){
    e.currentTarget.classList.remove('open');
    if(calFocusDk) setTimeout(()=>document.getElementById('calGrid').focus(), 50);
  }
});
// Esc inside memo modal input
document.getElementById('memoModalInput').addEventListener('keydown',e=>{
  if(e.key==='Enter') document.getElementById('memoModalAddBtn').click();
  if(e.key==='Escape'){
    document.getElementById('memoModal').classList.remove('open');
    if(calFocusDk) setTimeout(()=>document.getElementById('calGrid').focus(), 50);
  }
});

document.getElementById('calBtn').addEventListener('click',openCalendar);
document.getElementById('calBackBtn').addEventListener('click',closeCalendar);
document.getElementById('calPrevMonth').addEventListener('click',()=>{ calMonth--; if(calMonth<0){calMonth=11;calYear--;} renderCalendar(); });
document.getElementById('calNextMonth').addEventListener('click',()=>{ calMonth++; if(calMonth>11){calMonth=0;calYear++;} renderCalendar(); });

function renderCalendar(){
  const MONTHS=['Jan','Feb','Mar','Apr','May','Jun','Jul','Aug','Sep','Oct','Nov','Dec'];
  const DAYS=['Sun','Mon','Tue','Wed','Thu','Fri','Sat'];
  document.getElementById('calMonthLabel').textContent=`${MONTHS[calMonth]} ${calYear}`;

  const hdr=document.getElementById('calDayHeaders');
  hdr.innerHTML='';
  DAYS.forEach((d,i)=>{ hdr.innerHTML+=`<div class="cal-day-hdr${i===0||i===6?' weekend':''}">${d}</div>`; });

  const grid=document.getElementById('calGrid');
  grid.innerHTML='';

  const firstDay=new Date(calYear,calMonth,1).getDay();
  const daysInMonth=new Date(calYear,calMonth+1,0).getDate();
  const tk=todayKey();
  const now=new Date();
  const todayDate=new Date(now.getFullYear(),now.getMonth(),now.getDate());

  for(let i=0;i<firstDay;i++){
    const empty=document.createElement('div');
    empty.className='cal-cell cal-cell-empty';
    grid.appendChild(empty);
  }

  for(let d=1;d<=daysInMonth;d++){
    const dk=`${calYear}-${pad(calMonth+1)}-${pad(d)}`;
    const cellDate=new Date(calYear,calMonth,d);
    const isPast=cellDate<todayDate;
    const isToday=dk===tk;
    const notes=getNotes(dk);

    const cell=document.createElement('div');
    cell.className='cal-cell'+(isPast?' cal-cell-past':'')+(isToday?' cal-cell-today':'')+(notes.length?' cal-cell-has-memo':'');

    const dot=document.createElement('div'); dot.className='cal-memo-dot';
    const dateNum=document.createElement('div'); dateNum.className='cal-date-num'; dateNum.textContent=d;
    const memoList=document.createElement('div'); memoList.className='cal-memo-list';
    notes.slice(0,2).forEach(n=>{ const chip=document.createElement('div'); chip.className='cal-memo-chip'; chip.textContent=n; memoList.appendChild(chip); });
    if(notes.length>2){ const more=document.createElement('div'); more.className='cal-memo-chip'; more.style.color='var(--text-muted)'; more.textContent=`+${notes.length-2} more`; memoList.appendChild(more); }

    cell.appendChild(dot); cell.appendChild(dateNum); cell.appendChild(memoList);
    cell.dataset.dk=dk;
    if(!isPast) cell.addEventListener('click',()=>openMemoModal(dk));
    grid.appendChild(cell);
  }
  // restore keyboard focus ring if a date was focused
  if(calFocusDk) setCalFocus(calFocusDk);
}

// ── MEMO MODAL ──
let memoModalDk='';
function openMemoModal(dk){
  memoModalDk=dk;
  const [y,m,d]=dk.split('-').map(Number);
  const days=['Sun','Mon','Tue','Wed','Thu','Fri','Sat'];
  const dt=new Date(y,m-1,d);
  document.getElementById('memoModalDate').textContent=`${days[dt.getDay()]}, ${MONTHS_SHORT[m-1]} ${d}, ${y}`;
  renderMemoModalList();
  document.getElementById('memoModal').classList.add('open');
  setTimeout(()=>document.getElementById('memoModalInput').focus(),80);
}
function renderMemoModalList(){
  const notes=getNotes(memoModalDk);
  const list=document.getElementById('memoModalList');
  list.innerHTML='';
  if(!notes.length){ list.innerHTML='<div style="font-size:12px;color:var(--text-muted);padding:4px 0">No notes yet</div>'; return; }
  notes.forEach((n,i)=>{
    const item=document.createElement('div'); item.className='memo-modal-item';
    item.innerHTML=`<span class="memo-modal-text">${esc(n)}</span>`;
    const del=document.createElement('button'); del.className='memo-modal-del';
    del.innerHTML=SVG_X;
    del.addEventListener('click',()=>{ const arr=getNotes(memoModalDk); arr.splice(i,1); saveNotes(memoModalDk,arr); renderMemoModalList(); renderCalendar(); });
    item.appendChild(del); list.appendChild(item);
  });
}
document.getElementById('memoModalAddBtn').addEventListener('click',()=>{
  const val=document.getElementById('memoModalInput').value.trim();
  if(!val) return;
  const notes=getNotes(memoModalDk); notes.push(val); saveNotes(memoModalDk,notes);
  document.getElementById('memoModalInput').value='';
  renderMemoModalList(); renderCalendar();
});

// ══════════════════════════════════════
//  TOAST
// ══════════════════════════════════════
function showToast(msg){
  let t=document.getElementById('toast');
  if(!t){
    t=document.createElement('div'); t.id='toast';
    t.style.cssText='position:fixed;bottom:28px;left:50%;transform:translateX(-50%);background:#1E293B;color:#fff;font-size:13px;font-family:"Noto Sans KR",sans-serif;padding:9px 20px;border-radius:30px;z-index:9999;opacity:0;transition:opacity 0.2s;box-shadow:0 4px 16px rgba(0,0,0,0.2);pointer-events:none;white-space:nowrap';
    document.body.appendChild(t);
  }
  t.textContent=msg; t.style.opacity='1';
  clearTimeout(t._timer);
  t._timer=setTimeout(()=>{ t.style.opacity='0'; },2400);
}

// ══════════════════════════════════════
//  KEYBOARD NAVIGATION — BLOCKS
// ══════════════════════════════════════
//  KEYBOARD NAVIGATION — BLOCKS
// ══════════════════════════════════════
let kbBlockIdx = -1;   // focused block (-1 = none)
let kbRangeStart = -1; // shift-range anchor (-1 = not selecting)

function setKbBlockFocus(idx, keepRange){
  if(idx<0||idx>=TOTAL_BLOCKS) return;
  kbBlockIdx=idx;
  document.querySelectorAll('.block').forEach(b=>{
    const i=+b.dataset.idx;
    const inRange = kbRangeStart!==-1
      && i>=Math.min(kbRangeStart,kbBlockIdx)
      && i<=Math.max(kbRangeStart,kbBlockIdx);
    b.classList.toggle('kb-focus', i===kbBlockIdx && kbRangeStart===-1);
    b.classList.toggle('kb-range', inRange);
  });
  document.querySelector(`.block[data-idx="${idx}"]`)
    ?.scrollIntoView({block:'nearest',behavior:'smooth'});
}

function clearKbBlockFocus(){
  kbBlockIdx=-1; kbRangeStart=-1;
  document.querySelectorAll('.block').forEach(b=>
    b.classList.remove('kb-focus','kb-range'));
}

// Tab into block grid → jump to first block (6:00 :00)
document.getElementById('blockGrid').setAttribute('tabindex','-1');
document.getElementById('blockGrid').addEventListener('focus', e=>{
  if(kbBlockIdx===-1){ kbBlockIdx=0; setKbBlockFocus(0); }
});
document.getElementById('blockGrid').addEventListener('blur', e=>{
  if(!e.relatedTarget?.closest('#schedulePopup')) clearKbBlockFocus();
});

// mouse click also sets kb focus position
document.getElementById('blockGrid').addEventListener('mousedown', e=>{
  const b=e.target.closest('.block');
  if(b){ kbBlockIdx=+b.dataset.idx; kbRangeStart=-1; }
}, true);

document.getElementById('blockGrid').addEventListener('keydown', e=>{
  if(viewMode||kbBlockIdx===-1) return;
  const C=COLS;
  const arrows={ArrowRight:1, ArrowLeft:-1, ArrowDown:C, ArrowUp:-C};
  const delta=arrows[e.key];

  if(delta!==undefined){
    e.preventDefault();
    const next=kbBlockIdx+delta;
    if(next<0||next>=TOTAL_BLOCKS) return;

    if(e.shiftKey){
      // start or extend range selection
      if(kbRangeStart===-1) kbRangeStart=kbBlockIdx;
      kbBlockIdx=next;
      setKbBlockFocus(next);
    } else {
      // cancel any range and just move
      kbRangeStart=-1;
      setKbBlockFocus(next);
    }
    return;
  }

  if(e.key==='Escape'){
    e.preventDefault();
    kbRangeStart=-1;
    setKbBlockFocus(kbBlockIdx); // re-render: clears range highlight, keeps focus dot
    return;
  }

  // Space: fill / erase single focused block (only when no range active)
  if((e.key===' '||e.key==='Space') && kbRangeStart===-1){
    e.preventDefault();
    const el=document.querySelector(`.block[data-idx="${kbBlockIdx}"]`);
    if(el&&el.dataset.sched==='0'){
      const dk=todayKey(); const blocks=getBlocks(dk); const scMap=buildScMap(dk);
      if(blocks[kbBlockIdx]) eraseBlock(kbBlockIdx);
      else applyBlock(kbBlockIdx,true,PALETTE[getSelColor()],scMap);
    }
    return;
  }

  // Enter: open schedule popup for the current range (or single block)
  if(e.key==='Enter'){
    e.preventDefault();
    const lo=kbRangeStart!==-1 ? Math.min(kbRangeStart,kbBlockIdx) : kbBlockIdx;
    const hi=kbRangeStart!==-1 ? Math.max(kbRangeStart,kbBlockIdx) : kbBlockIdx;
    const saved=kbBlockIdx;
    kbRangeStart=-1;
    clearKbBlockFocus();
    // position popup next to the last focused block element
    const anchorEl=document.querySelector(`.block[data-idx="${hi}"]`);
    const rect=anchorEl ? anchorEl.getBoundingClientRect() : null;
    const fakeEv=rect
      ? {clientX: rect.right, clientY: rect.top + rect.height/2}
      : {clientX: window.innerWidth/2, clientY: window.innerHeight/2};
    openSchedulePopup(lo,hi,fakeEv);
    kbBlockIdx=saved;
    return;
  }
});

// ══════════════════════════════════════
//  KEYBOARD NAVIGATION — SCHEDULE LIST
// ══════════════════════════════════════
let schedFocusIdx = -1;

function renderSchedulesFocused(){
  document.querySelectorAll('.schedule-item').forEach((el,i)=>{
    el.classList.toggle('kb-focus', i===schedFocusIdx);
  });
}

function moveSchedFocus(dir){
  const items=document.querySelectorAll('.schedule-item');
  if(!items.length) return;
  schedFocusIdx=Math.max(0,Math.min(items.length-1,(schedFocusIdx<0?0:schedFocusIdx)+dir));
  renderSchedulesFocused();
  items[schedFocusIdx]?.scrollIntoView({block:'nearest'});
}

document.getElementById('scheduleList').addEventListener('keydown',e=>{
  if(viewMode) return;
  if(e.key==='ArrowDown'){ e.preventDefault(); moveSchedFocus(1); }
  else if(e.key==='ArrowUp'){ e.preventDefault(); moveSchedFocus(-1); }
  else if(e.key==='Enter' && schedFocusIdx>=0){
    e.preventDefault();
    const dk=todayKey();
    const item=document.querySelectorAll('.schedule-item')[schedFocusIdx];
    if(!item) return;
    const origIdx=+item.dataset.origIdx;
    const s=getSchedules(dk)[origIdx];
    if(!s) return;
    const rect=item.getBoundingClientRect();
    const ev=rect
      ? {clientX:rect.right, clientY:rect.top+rect.height/2}
      : {clientX:window.innerWidth/2, clientY:window.innerHeight/2};
    const lo=timeToBlock(s.start), hi=timeToBlock(s.end)-1;
    openSchedulePopup(lo, hi, ev, origIdx);
  }
  else if((e.key==='Delete'||e.key==='Backspace') && schedFocusIdx>=0){
    if(!document.getElementById('scheduleList').contains(document.activeElement) &&
       document.activeElement !== document.getElementById('scheduleList')) return;
    e.preventDefault();
    const dk=todayKey(); const all=getSchedules(dk);
    const item=document.querySelectorAll('.schedule-item')[schedFocusIdx];
    if(!item) return;
    const origIdx=+item.dataset.origIdx;
    const removed=all[origIdx];
    if(removed){
      const blocks=getBlocks(dk);
      const si=timeToBlock(removed.start), ei=timeToBlock(removed.end);
      for(let i=si;i<ei&&i<TOTAL_BLOCKS;i++) if(i>=0) delete blocks[i];
      saveBlocks(dk,blocks);
    }
    all.splice(origIdx,1); saveSchedules(dk,all);
    schedFocusIdx=Math.min(schedFocusIdx,all.length-1);
    renderSchedules(); renderBlocks(); renderSchedulesFocused();
  }
  else if(e.key==='Escape'){ schedFocusIdx=-1; renderSchedulesFocused(); document.getElementById('blockGrid').focus(); }
});

document.getElementById('scheduleList').setAttribute('tabindex','0');
document.getElementById('scheduleList').addEventListener('click',e=>{
  const item=e.target.closest('.schedule-item');
  if(item){
    schedFocusIdx=[...document.querySelectorAll('.schedule-item')].indexOf(item);
    renderSchedulesFocused();
  }
});

// ══════════════════════════════════════
//  GLOBAL SHORTCUTS
// ══════════════════════════════════════
document.addEventListener('keydown',e=>{
  const tag=document.activeElement?.tagName;
  const inInput=tag==='INPUT'||tag==='TEXTAREA';

  // ? — shortcut help (works everywhere except input)
  if(e.key==='?' && !inInput){
    e.preventDefault();
    document.getElementById('shortcutOverlay').classList.toggle('open');
    return;
  }
  if(inInput) return; // no other shortcuts while typing

  switch(e.key){
    case 'v': case 'V':
      e.preventDefault(); toggleViewMode(); break;
    case 'd': case 'D':
      e.preventDefault(); applyTheme(!isDark()); break;
    case 'b': case 'B':
      e.preventDefault();
      { const grid=document.getElementById('blockGrid');
        if(kbBlockIdx===-1) kbBlockIdx=0;
        setKbBlockFocus(kbBlockIdx);
        grid.focus(); }
      break;
    case 't': case 'T':
      e.preventDefault();
      document.getElementById('todoInput').focus();
      break;
    case 'c': case 'C':
      e.preventDefault(); openCalendar(); break;
    case 'p': case 'P':
      e.preventDefault(); closeCalendar(); break;
    case 's': case 'S':
      e.preventDefault();
      { const items=document.querySelectorAll('.schedule-item');
        if(!items.length){ showToast('No events yet'); break; }
        if(schedFocusIdx<0) schedFocusIdx=0;
        renderSchedulesFocused();
        document.getElementById('scheduleList').focus();
        items[schedFocusIdx]?.scrollIntoView({block:'nearest'}); }
      break;
    case 'r': case 'R':
      e.preventDefault(); document.getElementById('resetModal').classList.add('open'); break;
    case 'Escape':
      // close any open modal/popup
      document.getElementById('shortcutOverlay').classList.remove('open');
      document.getElementById('resetModal').classList.remove('open');
      document.getElementById('memoModal').classList.remove('open');
      closeSchedulePopup();
      break;
  }
});

document.getElementById('shortcutClose').addEventListener('click',()=>{
  document.getElementById('shortcutOverlay').classList.remove('open');
});
document.getElementById('shortcutOverlay').addEventListener('click',e=>{
  if(e.target===e.currentTarget) e.currentTarget.classList.remove('open');
});
// accordion toggle
document.querySelectorAll('.sc-cat-btn').forEach(btn=>{
  btn.addEventListener('click',()=>{
    const cat=btn.closest('.sc-cat');
    const wasOpen=cat.classList.contains('open');
    document.querySelectorAll('.sc-cat').forEach(c=>c.classList.remove('open'));
    if(!wasOpen) cat.classList.add('open');
  });
});

// ── also re-apply schedule focus ring after re-render ──
const _origRenderSchedules = renderSchedules;
renderSchedules = function(){
  _origRenderSchedules();
  renderSchedulesFocused();
};

// ══════════════════════════════════════
//  AUTH UI
// ══════════════════════════════════════
let authMode = 'login'; // 'login' | 'signup'

document.getElementById('tabLogin').addEventListener('click',()=>{
  authMode='login';
  document.getElementById('tabLogin').classList.add('active');
  document.getElementById('tabSignup').classList.remove('active');
  document.getElementById('authSubmit').textContent='Sign in';
  document.getElementById('authError').textContent='';
});
document.getElementById('tabSignup').addEventListener('click',()=>{
  authMode='signup';
  document.getElementById('tabSignup').classList.add('active');
  document.getElementById('tabLogin').classList.remove('active');
  document.getElementById('authSubmit').textContent='Sign up';
  document.getElementById('authError').textContent='';
});

document.getElementById('authSubmit').addEventListener('click', handleAuth);
document.getElementById('authPassword').addEventListener('keydown',e=>{ if(e.key==='Enter') handleAuth(); });

async function handleAuth(){
  const email    = document.getElementById('authEmail').value.trim();
  const password = document.getElementById('authPassword').value;
  const errEl    = document.getElementById('authError');
  const btn      = document.getElementById('authSubmit');
  if(!email||!password){ errEl.textContent='Please fill in all fields.'; return; }
  btn.textContent='...'; btn.disabled=true; errEl.textContent='';
  let error;
  if(authMode==='login'){
    ({ error } = await sb.auth.signInWithPassword({ email, password }));
  } else {
    ({ error } = await sb.auth.signUp({ email, password }));
    if(!error) errEl.style.color='var(--blue-600)', errEl.textContent='Check your email to confirm your account!';
  }
  btn.disabled=false;
  btn.textContent = authMode==='login'?'Sign in':'Sign up';
  if(error) errEl.textContent=error.message;
}

document.getElementById('logoutBtn').addEventListener('click',async()=>{
  await sb.auth.signOut();
});

function showAuthView(){
  document.getElementById('authView').classList.add('active');
  document.getElementById('plannerView').style.display='none';
  document.getElementById('calendarView').classList.remove('active');
}

function showPlannerView(){
  document.getElementById('authView').classList.remove('active');
  document.getElementById('plannerView').style.display='block';
}

// ══════════════════════════════════════
//  INIT
// ══════════════════════════════════════
applyTheme(!!get('bp_dark'));

let nowBlockTimer = null;

function startNowBlockTimer(){
  if(nowBlockTimer) clearInterval(nowBlockTimer);
  // align to next full minute for accuracy
  const msToNextMinute = (60 - new Date().getSeconds()) * 1000;
  setTimeout(()=>{
    renderBlocks();
    nowBlockTimer = setInterval(()=>{ renderBlocks(); }, 60000);
  }, msToNextMinute);
}

let plannerInitialized = false;

async function initPlanner(user){
  currentUser = user;
  document.getElementById('userBadge').textContent = currentUser.email;
  showPlannerView();
  document.getElementById('dateDisplayStatic').textContent=formatDate(todayKey());
  // 즉시 빈 화면 렌더링 (빠른 진입)
  await new Promise(r => requestAnimationFrame(r));
  renderTimeLabels();
  renderBlocks();
  renderSchedules();
  renderTodos();
  startNowBlockTimer();
  plannerInitialized = true;
  // 백그라운드에서 데이터 로드 후 화면 갱신
  loadRemoteData().then(()=>{
    renderBlocks();
    renderSchedules();
    renderTodos();
  });
}

// listen to auth state changes (handles login/logout after initial load)
sb.auth.onAuthStateChange(async (event, session)=>{
  if(event==='SIGNED_IN' && session?.user && !plannerInitialized){
    await initPlanner(session.user);
  } else if(event==='SIGNED_OUT'){
    currentUser = null;
    plannerInitialized = false;
    remoteData = { blocks:{}, schedules:{}, notes:{}, todos:[] };
    if(nowBlockTimer){ clearInterval(nowBlockTimer); nowBlockTimer=null; }
    showAuthView();
  }
});

// check existing session on load (handles refresh)
const { data:{ session } } = await sb.auth.getSession();
if(session?.user){
  await initPlanner(session.user);
} else {
  showAuthView();
}

</script>
</body>
</html>
