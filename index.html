import { useState, useRef } from “react”;

/* ─── GLOBAL STYLES ─────────────────────────────────────────────────────── */
const G = `@import url('https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=JetBrains+Mono:wght@400;600&display=swap'); *,*::before,*::after{box-sizing:border-box;margin:0;padding:0;} :root{ --bg:#06080f;--s1:#0c1018;--s2:#101520;--border:#1c2535; --a:#00e5ff;--a2:#ff5e3a;--a3:#b8ff57; --text:#ddeeff;--muted:#3d5570;--glow:rgba(0,229,255,.14);--glow2:rgba(255,94,58,.12); } body{font-family:'Syne',sans-serif;background:var(--bg);color:var(--text);min-height:100vh;overflow-x:hidden;} ::-webkit-scrollbar{width:4px}::-webkit-scrollbar-track{background:transparent}::-webkit-scrollbar-thumb{background:var(--border);border-radius:2px} .mono{font-family:'JetBrains Mono',monospace;} .dot{width:8px;height:8px;border-radius:50%;background:var(--muted);transition:all .3s;} .dot.on{background:var(--a3);box-shadow:0 0 8px var(--a3);} .dot.ing{background:var(--a);box-shadow:0 0 8px var(--a);animation:blink 1s infinite;} .dot.err{background:var(--a2);box-shadow:0 0 8px var(--a2);} @keyframes blink{0%,100%{opacity:1}50%{opacity:.25}} .badge{display:inline-flex;align-items:center;padding:2px 8px;border-radius:4px;font-size:10px;font-weight:700;letter-spacing:1px;text-transform:uppercase;} .b-green{background:rgba(184,255,87,.1);color:var(--a3);border:1px solid rgba(184,255,87,.25);} .b-red{background:rgba(255,94,58,.1);color:var(--a2);border:1px solid rgba(255,94,58,.25);} .b-blue{background:rgba(0,229,255,.1);color:var(--a);border:1px solid rgba(0,229,255,.25);} .b-grey{background:rgba(60,80,110,.2);color:var(--muted);border:1px solid var(--border);} .notif{position:fixed;top:80px;right:24px;z-index:900;background:var(--s2);border:1px solid var(--border);border-radius:12px;padding:14px 18px;display:flex;align-items:center;gap:10px;font-size:13px;max-width:310px;box-shadow:0 8px 32px rgba(0,0,0,.6);animation:slideR .3s ease;} .notif.success{border-color:var(--a3);}.notif.error{border-color:var(--a2);}.notif.info{border-color:var(--a);} @keyframes slideR{from{transform:translateX(110%);opacity:0}to{transform:translateX(0);opacity:1}} .hdr{display:flex;align-items:center;justify-content:space-between;padding:16px 32px;border-bottom:1px solid var(--border);background:rgba(12,16,24,.9);backdrop-filter:blur(20px);position:sticky;top:0;z-index:200;} .logo{display:flex;align-items:center;gap:11px;cursor:pointer;} .logo-box{width:34px;height:34px;border-radius:8px;background:linear-gradient(135deg,var(--a),#0088aa);display:flex;align-items:center;justify-content:center;font-size:17px;box-shadow:0 0 18px var(--glow);} .logo-name{font-size:18px;font-weight:800;letter-spacing:2px;text-transform:uppercase;background:linear-gradient(90deg,var(--a),#fff);-webkit-background-clip:text;-webkit-text-fill-color:transparent;} .hdr-right{display:flex;align-items:center;gap:14px;} .hdr-status{display:flex;align-items:center;gap:7px;font-size:12px;color:var(--muted);} .hdr-status span{font-family:'JetBrains Mono',monospace;} .btn-sm{padding:7px 16px;border-radius:7px;border:1px solid var(--border);background:transparent;color:var(--muted);font-family:'Syne',sans-serif;font-size:12px;font-weight:700;letter-spacing:.5px;cursor:pointer;transition:all .2s;} .btn-sm:hover{color:var(--text);border-color:var(--a);} .btn-sm.danger{border-color:rgba(255,94,58,.35);color:var(--a2);} .btn-sm.danger:hover{background:rgba(255,94,58,.1);} @keyframes fadeUp{from{transform:translateY(24px);opacity:0}to{transform:translateY(0);opacity:1}} .home{min-height:calc(100vh - 67px);display:flex;flex-direction:column;align-items:center;justify-content:center;padding:60px 24px;position:relative;overflow:hidden;} .home-ring{position:absolute;border-radius:50%;border:1px solid;animation:expand 6s ease-out infinite;pointer-events:none;} .home-ring:nth-child(1){width:400px;height:400px;border-color:rgba(0,229,255,.06);animation-delay:0s;} .home-ring:nth-child(2){width:650px;height:650px;border-color:rgba(0,229,255,.04);animation-delay:1.5s;} .home-ring:nth-child(3){width:900px;height:900px;border-color:rgba(0,229,255,.025);animation-delay:3s;} @keyframes expand{0%{transform:scale(.7);opacity:0}40%{opacity:1}100%{transform:scale(1.15);opacity:0}} .home-glow{position:absolute;top:50%;left:50%;transform:translate(-50%,-50%);width:600px;height:600px;border-radius:50%;background:radial-gradient(circle,rgba(0,229,255,.05) 0%,transparent 70%);pointer-events:none;} .home-hero{text-align:center;margin-bottom:60px;position:relative;z-index:1;animation:fadeUp .7s ease both;} .hero-icon{width:80px;height:80px;border-radius:20px;margin:0 auto 24px;background:linear-gradient(135deg,rgba(0,229,255,.15),rgba(0,229,255,.04));border:1px solid rgba(0,229,255,.25);display:flex;align-items:center;justify-content:center;font-size:36px;box-shadow:0 0 40px var(--glow),inset 0 0 30px rgba(0,229,255,.05);} .hero-title{font-size:48px;font-weight:800;letter-spacing:-1px;background:linear-gradient(160deg,#fff 30%,var(--a) 100%);-webkit-background-clip:text;-webkit-text-fill-color:transparent;margin-bottom:12px;} .hero-sub{font-size:15px;color:var(--muted);max-width:380px;margin:0 auto;line-height:1.7;font-weight:400;} .conn-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;max-width:820px;width:100%;position:relative;z-index:1;animation:fadeUp .7s .2s ease both;} .conn-card{background:var(--s1);border:1px solid var(--border);border-radius:18px;padding:32px 28px;cursor:pointer;transition:all .25s cubic-bezier(.2,.8,.3,1);display:flex;flex-direction:column;align-items:flex-start;gap:16px;position:relative;overflow:hidden;} .conn-card::after{content:'';position:absolute;inset:0;border-radius:18px;background:linear-gradient(135deg,rgba(0,229,255,.05),transparent);opacity:0;transition:opacity .25s;} .conn-card:hover{transform:translateY(-4px);box-shadow:0 16px 48px rgba(0,0,0,.5);} .conn-card:hover::after{opacity:1;} .conn-card.m3u:hover{border-color:var(--a);box-shadow:0 16px 48px rgba(0,0,0,.5),0 0 30px var(--glow);} .conn-card.xtream:hover{border-color:var(--a2);box-shadow:0 16px 48px rgba(0,0,0,.5),0 0 30px var(--glow2);} .conn-card.stalker:hover{border-color:var(--a3);box-shadow:0 16px 48px rgba(0,0,0,.5),0 0 30px rgba(184,255,87,.12);} .card-icon{width:52px;height:52px;border-radius:13px;display:flex;align-items:center;justify-content:center;font-size:24px;border:1px solid;} .icon-blue{background:rgba(0,229,255,.1);border-color:rgba(0,229,255,.25);} .icon-orange{background:rgba(255,94,58,.1);border-color:rgba(255,94,58,.25);} .icon-green{background:rgba(184,255,87,.1);border-color:rgba(184,255,87,.25);} .card-label{font-size:11px;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--muted);} .card-name{font-size:20px;font-weight:800;margin-top:-4px;} .card-desc{font-size:13px;color:var(--muted);line-height:1.6;font-weight:400;} .card-arrow{margin-top:auto;align-self:flex-end;width:32px;height:32px;border-radius:50%;background:var(--border);display:flex;align-items:center;justify-content:center;font-size:14px;color:var(--muted);transition:all .2s;} .conn-card:hover .card-arrow{color:#000;} .conn-card.m3u:hover .card-arrow{background:var(--a);} .conn-card.xtream:hover .card-arrow{background:var(--a2);} .conn-card.stalker:hover .card-arrow{background:var(--a3);} .saved-strip{max-width:820px;width:100%;margin-top:40px;position:relative;z-index:1;animation:fadeUp .7s .35s ease both;} .strip-label{font-size:11px;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--muted);margin-bottom:14px;} .strip-row{display:flex;gap:10px;flex-wrap:wrap;} .saved-pill{display:flex;align-items:center;gap:10px;background:var(--s1);border:1px solid var(--border);border-radius:50px;padding:8px 16px 8px 10px;cursor:pointer;transition:all .2s;} .saved-pill:hover{border-color:var(--a);background:rgba(0,229,255,.05);} .pill-icon{width:28px;height:28px;border-radius:50%;background:var(--s2);display:flex;align-items:center;justify-content:center;font-size:13px;} .pill-name{font-size:13px;font-weight:600;} .pill-host{font-family:'JetBrains Mono',monospace;font-size:10px;color:var(--muted);} .form-screen{min-height:calc(100vh - 67px);display:flex;align-items:center;justify-content:center;padding:40px 24px;} .form-card{background:var(--s1);border:1px solid var(--border);border-radius:20px;padding:40px 44px;width:100%;max-width:520px;animation:fadeUp .5s ease both;} .form-back{display:flex;align-items:center;gap:8px;font-size:12px;font-weight:700;letter-spacing:1px;text-transform:uppercase;color:var(--muted);cursor:pointer;margin-bottom:32px;transition:color .2s;width:fit-content;} .form-back:hover{color:var(--text);} .form-header{display:flex;align-items:center;gap:16px;margin-bottom:32px;} .form-icon{width:48px;height:48px;border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:22px;border:1px solid;} .form-title{font-size:22px;font-weight:800;} .form-sub{font-size:13px;color:var(--muted);font-weight:400;margin-top:3px;} .fields{display:flex;flex-direction:column;gap:16px;} .field{display:flex;flex-direction:column;gap:7px;} .field label{font-size:11px;font-weight:700;letter-spacing:1.5px;text-transform:uppercase;color:var(--muted);} .field input,.field select{background:var(--s2);border:1px solid var(--border);border-radius:10px;color:var(--text);font-family:'JetBrains Mono',monospace;font-size:13px;padding:12px 16px;outline:none;transition:all .2s;-webkit-appearance:none;} .field input:focus,.field select:focus{border-color:var(--a);box-shadow:0 0 0 3px var(--glow);} .field input::placeholder{color:var(--muted);} .field select option{background:var(--s2);} .row2{display:grid;grid-template-columns:1fr 1fr;gap:12px;} .divider{height:1px;background:var(--border);margin:4px 0;} .btn-connect{width:100%;padding:14px;border-radius:10px;border:none;background:linear-gradient(135deg,var(--a),#0099bb);color:#000;font-family:'Syne',sans-serif;font-size:14px;font-weight:800;letter-spacing:1px;text-transform:uppercase;cursor:pointer;transition:all .2s;margin-top:4px;box-shadow:0 4px 24px rgba(0,229,255,.3);} .btn-connect:hover:not(:disabled){transform:translateY(-1px);box-shadow:0 6px 32px rgba(0,229,255,.45);} .btn-connect:disabled{opacity:.45;cursor:not-allowed;transform:none;} .btn-connect.orange{background:linear-gradient(135deg,var(--a2),#cc3300);box-shadow:0 4px 24px rgba(255,94,58,.3);} .btn-connect.orange:hover:not(:disabled){box-shadow:0 6px 32px rgba(255,94,58,.45);} .btn-connect.green{background:linear-gradient(135deg,var(--a3),#66cc00);box-shadow:0 4px 24px rgba(184,255,87,.3);} .btn-connect.green:hover:not(:disabled){box-shadow:0 6px 32px rgba(184,255,87,.45);} .log-box{background:var(--bg);border:1px solid var(--border);border-radius:8px;padding:12px;overflow-y:auto;display:flex;flex-direction:column;gap:3px;font-family:'JetBrains Mono',monospace;font-size:11px;} .log-row{display:flex;gap:8px;} .lt{color:var(--muted);flex-shrink:0;}.li{color:var(--a);}.lo{color:var(--a3);}.le{color:var(--a2);}.lw{color:#ffaa44;} .app-layout{display:grid;grid-template-columns:300px 1fr;height:calc(100vh - 67px);overflow:hidden;} .sb{border-right:1px solid var(--border);background:var(--s1);display:flex;flex-direction:column;overflow-y:auto;} .sb-sec{padding:22px;border-bottom:1px solid var(--border);} .sb-label{font-size:10px;font-weight:700;letter-spacing:2.5px;text-transform:uppercase;color:var(--muted);margin-bottom:14px;} .srv-info{background:var(--s2);border:1px solid var(--border);border-radius:12px;padding:14px 16px;} .srv-row{display:flex;align-items:center;justify-content:space-between;margin-bottom:8px;} .srv-name{font-size:14px;font-weight:700;} .srv-meta{display:flex;flex-direction:column;gap:4px;font-family:'JetBrains Mono',monospace;font-size:10px;color:var(--muted);} .srv-badges{display:flex;gap:5px;margin-top:8px;flex-wrap:wrap;} .stats{display:grid;grid-template-columns:1fr 1fr 1fr;gap:8px;margin-top:14px;} .stat{background:var(--s2);border:1px solid var(--border);border-radius:9px;padding:11px;text-align:center;} .stat-val{font-size:18px;font-weight:800;color:var(--a);} .stat-key{font-size:10px;color:var(--muted);text-transform:uppercase;letter-spacing:1px;margin-top:2px;} .srv-list{display:flex;flex-direction:column;gap:7px;} .srv-item{background:var(--s2);border:1px solid var(--border);border-radius:10px;padding:11px 13px;cursor:pointer;transition:all .2s;display:flex;align-items:center;justify-content:space-between;} .srv-item:hover{border-color:var(--a);} .srv-item-name{font-size:13px;font-weight:600;} .srv-item-url{font-family:'JetBrains Mono',monospace;font-size:10px;color:var(--muted);margin-top:2px;} .srv-item-badges{display:flex;gap:4px;margin-top:5px;} .content{display:flex;flex-direction:column;overflow:hidden;} .content-hdr{padding:18px 28px;border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between;flex-shrink:0;} .ch-title{font-size:17px;font-weight:800;} .ch-sub{font-size:11px;color:var(--muted);margin-top:3px;font-family:'JetBrains Mono',monospace;} .search{background:var(--s2);border:1px solid var(--border);border-radius:8px;color:var(--text);font-family:'Syne',sans-serif;font-size:13px;padding:8px 14px;outline:none;width:210px;transition:all .2s;} .search:focus{border-color:var(--a);box-shadow:0 0 0 3px var(--glow);} .search::placeholder{color:var(--muted);} .tabs{display:flex;gap:6px;padding:16px 28px 0;flex-wrap:wrap;} .tab{padding:6px 15px;border-radius:20px;font-size:12px;font-weight:700;letter-spacing:.5px;cursor:pointer;border:1px solid var(--border);background:transparent;color:var(--muted);transition:all .2s;} .tab:hover{color:var(--text);border-color:var(--a);} .tab.act{background:var(--a);color:#000;border-color:var(--a);box-shadow:0 0 14px var(--glow);} .ch-area{flex:1;overflow-y:auto;padding:20px 28px;} .ch-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(170px,1fr));gap:12px;} .ch-card{background:var(--s2);border:1px solid var(--border);border-radius:13px;padding:18px 14px;cursor:pointer;transition:all .25s;display:flex;flex-direction:column;align-items:center;gap:9px;text-align:center;position:relative;overflow:hidden;} .ch-card::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;background:linear-gradient(90deg,transparent,var(--a),transparent);opacity:0;transition:opacity .2s;} .ch-card:hover{border-color:var(--a);transform:translateY(-2px);box-shadow:0 8px 28px rgba(0,0,0,.4),0 0 18px var(--glow);} .ch-card:hover::before{opacity:1;} .ch-card.live{border-color:var(--a3);box-shadow:0 0 18px rgba(184,255,87,.15);} .ch-logo{width:54px;height:54px;border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:25px;} .ch-name{font-size:13px;font-weight:700;line-height:1.3;} .ch-group{font-size:10px;color:var(--muted);text-transform:uppercase;letter-spacing:1px;} .live-bar{position:absolute;bottom:0;left:0;right:0;height:3px;background:var(--a3);transform-origin:left;animation:prog 8s linear infinite;} @keyframes prog{from{transform:scaleX(0)}to{transform:scaleX(1)}} .player{border-top:1px solid var(--border);background:var(--s1);padding:13px 28px;display:flex;align-items:center;gap:18px;flex-shrink:0;} .pl-ch{display:flex;align-items:center;gap:11px;min-width:190px;} .pl-logo{width:34px;height:34px;border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:16px;} .pl-name{font-size:13px;font-weight:700;} .pl-live{font-size:11px;color:var(--a3);display:flex;align-items:center;gap:5px;margin-top:2px;} .pl-ctrls{display:flex;align-items:center;gap:10px;} .ctrl{width:34px;height:34px;border-radius:50%;background:var(--s2);border:1px solid var(--border);color:var(--text);font-size:14px;cursor:pointer;display:flex;align-items:center;justify-content:center;transition:all .2s;} .ctrl:hover{border-color:var(--a);color:var(--a);} .ctrl.act{background:var(--a);color:#000;border-color:var(--a);} .pl-right{margin-left:auto;display:flex;align-items:center;gap:14px;} .q-badge{padding:4px 10px;border-radius:6px;font-size:11px;font-weight:700;letter-spacing:1px;background:rgba(0,229,255,.1);color:var(--a);border:1px solid rgba(0,229,255,.22);} .sig{display:flex;align-items:flex-end;gap:2px;height:18px;} .sig span{width:3px;border-radius:2px;background:var(--a3);} .empty{display:flex;flex-direction:column;align-items:center;justify-content:center;height:100%;gap:14px;color:var(--muted);text-align:center;padding:60px;} .empty-ico{font-size:56px;opacity:.25;} .empty-t{font-size:18px;font-weight:700;color:var(--text);opacity:.4;} .empty-s{font-size:14px;max-width:280px;line-height:1.7;}`;

const CHANNELS = [
{id:1,name:“CNN International”,group:“News”,emoji:“📺”,color:”#cc0000”,quality:“HD”},
{id:2,name:“BBC World News”,group:“News”,emoji:“🇬🇧”,color:”#bb1919”,quality:“FHD”},
{id:3,name:“Al Jazeera”,group:“News”,emoji:“🌍”,color:”#cc6600”,quality:“HD”},
{id:4,name:“Eurosport 1”,group:“Sports”,emoji:“⚽”,color:”#004499”,quality:“4K”},
{id:5,name:“Sky Sports”,group:“Sports”,emoji:“🏆”,color:”#0066cc”,quality:“FHD”},
{id:6,name:“DAZN”,group:“Sports”,emoji:“🥊”,color:”#ffcc00”,quality:“4K”},
{id:7,name:“HBO”,group:“Entertainment”,emoji:“🎬”,color:”#6600cc”,quality:“4K”},
{id:8,name:“Prime Video”,group:“Entertainment”,emoji:“🎭”,color:”#00a8e0”,quality:“FHD”},
{id:9,name:“Discovery”,group:“Doku”,emoji:“🔬”,color:”#009933”,quality:“FHD”},
{id:10,name:“National Geo”,group:“Doku”,emoji:“🌿”,color:”#ffaa00”,quality:“HD”},
{id:11,name:“MTV Europe”,group:“Musik”,emoji:“🎵”,color:”#ff0099”,quality:“HD”},
{id:12,name:“Cartoon Network”,group:“Kids”,emoji:“🎨”,color:”#ff6600”,quality:“FHD”},
];

const SAVED = [
{id:1,name:“Mein Heimserver”,host:“iptv.home.local”,port:“8080”,type:“Xtream”,status:“online”,channels:432,emoji:“🏠”},
{id:2,name:“Premium Sports”,host:“sports.iptv.net”,port:“80”,type:“M3U”,status:“offline”,channels:87,emoji:“⚽”},
{id:3,name:“Family Pack”,host:“family.streams.tv”,port:“443”,type:“Stalker”,status:“online”,channels:210,emoji:“👨‍👩‍👧”},
];

const CATS = [“Alle”,“News”,“Sports”,“Entertainment”,“Doku”,“Musik”,“Kids”];

const CONN_TYPES = [
{key:“M3U”,label:“Playlist”,name:“M3U URL”,desc:“Direkte M3U-Playlist-URL deines Anbieters — einfachste Methode.”,emoji:“📋”,iconClass:“icon-blue”,cardClass:“m3u”,btnClass:””},
{key:“Xtream”,label:“API”,name:“Xtream Codes”,desc:“Login mit Benutzername & Passwort über die Xtream Codes API.”,emoji:“⚡”,iconClass:“icon-orange”,cardClass:“xtream”,btnClass:“orange”},
{key:“Stalker”,label:“Portal”,name:“Stalker Portal”,desc:“MAC-Adresse-basierter Zugang über ein Stalker-Middleware-Portal.”,emoji:“🔮”,iconClass:“icon-green”,cardClass:“stalker”,btnClass:“green”},
];

const delay = ms => new Promise(r=>setTimeout(r,ms));

export default function App() {
const [page, setPage] = useState(“home”);
const [connType, setConnType] = useState(null);
const [form, setForm] = useState({name:””,host:””,port:“8080”,user:””,pass:””,url:””,mac:””});
const [status, setStatus] = useState(“off”);
const [activeServer, setActiveServer] = useState(null);
const [cat, setCat] = useState(“Alle”);
const [search, setSearch] = useState(””);
const [playing, setPlaying] = useState(null);
const [paused, setPaused] = useState(false);
const [logs, setLogs] = useState([{t:“info”,m:“IPTV Client bereit”,ts:“00:00:00”}]);
const [notif, setNotif] = useState(null);
const logRef = useRef();

const addLog = (m,t=“info”) => {
const now=new Date();
const ts=[now.getHours(),now.getMinutes(),now.getSeconds()].map(n=>String(n).padStart(2,‘0’)).join(’:’);
setLogs(l=>[…l.slice(-60),{t,m,ts}]);
setTimeout(()=>{if(logRef.current)logRef.current.scrollTop=9999;},40);
};

const toast = (msg,type=“info”) => {setNotif({msg,type});setTimeout(()=>setNotif(null),3400);};

const openForm = (ct) => {setConnType(ct);setForm({name:””,host:””,port:“8080”,user:””,pass:””,url:””,mac:””});setPage(“form”);};

const connect = async () => {
const target = connType.key===“M3U”?form.url:form.host;
if(!target){toast(“Bitte Server-Adresse eingeben”,“error”);return;}
setStatus(“ing”);
addLog(`[${connType.key}] Verbindung wird aufgebaut...`,“info”);
await delay(700); addLog(“TCP-Handshake…”,“info”);
await delay(600); addLog(“Protokoll wird ausgehandelt…”,“info”);
await delay(500); addLog(connType.key===“Xtream”?“Anmeldedaten werden geprüft…”:“Playlist wird abgerufen…”,“info”);
await delay(700); addLog(`${CHANNELS.length} Kanäle empfangen.`,“ok”);
setStatus(“on”);
const srv={name:form.name||target,host:form.host||form.url,port:form.port,type:connType.key,channels:CHANNELS.length,emoji:connType.emoji};
setActiveServer(srv);
setPage(“app”);
toast(`✓ Verbunden mit ${srv.name}`,“success”);
};

const connectSaved = async (s) => {
if(s.status===“offline”){toast(“Server ist offline”,“error”);return;}
setStatus(“ing”);
addLog(`Verbinde mit: ${s.name}...`,“info”);
await delay(1100);
addLog(`${s.channels} Kanäle geladen.`,“ok”);
setStatus(“on”);
setActiveServer(s);
setPage(“app”);
toast(`✓ Verbunden mit ${s.name}`,“success”);
};

const disconnect = () => {
setStatus(“off”);setActiveServer(null);setPlaying(null);setPage(“home”);
addLog(“Verbindung getrennt.”,“warn”);
toast(“Verbindung getrennt”,“info”);
};

const filteredCh = CHANNELS.filter(c=>(cat===“Alle”||c.group===cat)&&c.name.toLowerCase().includes(search.toLowerCase()));
const statusTxt={off:“Nicht verbunden”,ing:“Verbinde…”,on:“Verbunden”,err:“Fehler”}[status];
const ct = connType||CONN_TYPES[0];

return (
<>
<style>{G}</style>

```
  {notif&&(
    <div className={`notif ${notif.type}`}>
      <span>{notif.type==="success"?"✓":notif.type==="error"?"✗":"ℹ"}</span>
      {notif.msg}
    </div>
  )}

  <header className="hdr">
    <div className="logo" onClick={()=>{if(status!=="on")setPage("home");}}>
      <div className="logo-box">📡</div>
      <div className="logo-name">IPTV Pro</div>
    </div>
    <div className="hdr-right">
      <div className="hdr-status">
        <div className={`dot ${status==="on"?"on":status==="ing"?"ing":""}`}/>
        <span>{statusTxt}</span>
        {activeServer&&<span style={{color:"var(--text)",marginLeft:4}}>— {activeServer.name}</span>}
      </div>
      {page==="form"&&<button className="btn-sm" onClick={()=>setPage("home")}>← Zurück</button>}
      {status==="on"&&<button className="btn-sm danger" onClick={disconnect}>⏻ Trennen</button>}
    </div>
  </header>

  {/* HOME */}
  {page==="home"&&(
    <div className="home">
      <div className="home-ring"/><div className="home-ring"/><div className="home-ring"/>
      <div className="home-glow"/>
      <div className="home-hero">
        <div className="hero-icon">📡</div>
        <div className="hero-title">IPTV Pro</div>
        <div className="hero-sub">Wähle deinen Verbindungstyp, um mit deinem IPTV-Server zu verbinden.</div>
      </div>
      <div className="conn-grid">
        {CONN_TYPES.map(ct=>(
          <div key={ct.key} className={`conn-card ${ct.cardClass}`} onClick={()=>openForm(ct)}>
            <div className={`card-icon ${ct.iconClass}`}>{ct.emoji}</div>
            <div>
              <div className="card-label">{ct.label}</div>
              <div className="card-name">{ct.name}</div>
            </div>
            <div className="card-desc">{ct.desc}</div>
            <div className="card-arrow">›</div>
          </div>
        ))}
      </div>
      <div className="saved-strip">
        <div className="strip-label">📌 Gespeicherte Server</div>
        <div className="strip-row">
          {SAVED.map(s=>(
            <div key={s.id} className="saved-pill" onClick={()=>connectSaved(s)}>
              <div className="pill-icon">{s.emoji}</div>
              <div>
                <div className="pill-name">{s.name}</div>
                <div className="pill-host">{s.host}</div>
              </div>
              <span className={`badge ${s.status==="online"?"b-green":"b-red"}`} style={{marginLeft:4}}>{s.status}</span>
            </div>
          ))}
        </div>
      </div>
    </div>
  )}

  {/* FORM */}
  {page==="form"&&(
    <div className="form-screen">
      <div className="form-card">
        <div className="form-back" onClick={()=>setPage("home")}>← Verbindungsauswahl</div>
        <div className="form-header">
          <div className={`form-icon ${ct.iconClass}`}>{ct.emoji}</div>
          <div>
            <div className="form-title">{ct.name}</div>
            <div className="form-sub">{ct.desc}</div>
          </div>
        </div>
        <div className="fields">
          {ct.key==="M3U"&&(
            <div className="field">
              <label>Playlist-URL *</label>
              <input placeholder="http://server.com/get.php?username=...&type=m3u" value={form.url} onChange={e=>setForm(f=>({...f,url:e.target.value}))}/>
            </div>
          )}
          {ct.key==="Xtream"&&(<>
            <div className="row2">
              <div className="field"><label>Host *</label><input placeholder="iptv.server.com" value={form.host} onChange={e=>setForm(f=>({...f,host:e.target.value}))}/></div>
              <div className="field"><label>Port</label><input placeholder="8080" value={form.port} onChange={e=>setForm(f=>({...f,port:e.target.value}))}/></div>
            </div>
            <div className="row2">
              <div className="field"><label>Benutzername *</label><input placeholder="user123" value={form.user} onChange={e=>setForm(f=>({...f,user:e.target.value}))}/></div>
              <div className="field"><label>Passwort *</label><input type="password" placeholder="••••••" value={form.pass} onChange={e=>setForm(f=>({...f,pass:e.target.value}))}/></div>
            </div>
          </>)}
          {ct.key==="Stalker"&&(<>
            <div className="field"><label>Portal-URL *</label><input placeholder="http://portal.iptv.com/stalker_portal/c/" value={form.host} onChange={e=>setForm(f=>({...f,host:e.target.value}))}/></div>
            <div className="field"><label>MAC-Adresse *</label><input placeholder="00:1A:79:XX:XX:XX" value={form.mac} onChange={e=>setForm(f=>({...f,mac:e.target.value}))}/></div>
          </>)}
          <div className="divider"/>
          <div className="field">
            <label>Anzeigename (optional)</label>
            <input placeholder="z.B. Mein Heimserver" value={form.name} onChange={e=>setForm(f=>({...f,name:e.target.value}))}/>
          </div>
          {logs.length>1&&(
            <div className="log-box" ref={logRef} style={{height:100}}>
              {logs.map((l,i)=>(
                <div key={i} className="log-row">
                  <span className="lt">{l.ts}</span>
                  <span className={l.t==="ok"?"lo":l.t==="error"?"le":l.t==="warn"?"lw":"li"}>{l.m}</span>
                </div>
              ))}
            </div>
          )}
          <button className={`btn-connect ${ct.btnClass}`} onClick={connect} disabled={status==="ing"}>
            {status==="ing"?"⏳ Verbinde…":`⚡ Mit ${ct.name} verbinden`}
          </button>
        </div>
      </div>
    </div>
  )}

  {/* APP */}
  {page==="app"&&(
    <div className="app-layout">
      <aside className="sb">
        <div className="sb-sec">
          <div className="sb-label">🔌 Aktiver Server</div>
          <div className="srv-info">
            <div className="srv-row">
              <div className="srv-name">{activeServer?.name}</div>
              <div className="dot on"/>
            </div>
            <div className="srv-meta">
              <span>{activeServer?.host}{activeServer?.port?`:${activeServer.port}`:""}</span>
            </div>
            <div className="srv-badges">
              <span className="badge b-green">Online</span>
              <span className="badge b-blue">{activeServer?.type}</span>
              <span className="badge b-grey">{activeServer?.channels} CH</span>
            </div>
          </div>
          <div className="stats">
            <div className="stat"><div className="stat-val">{CHANNELS.length}</div><div className="stat-key">Kanäle</div></div>
            <div className="stat"><div className="stat-val">7</div><div className="stat-key">Gruppen</div></div>
            <div className="stat"><div className="stat-val" style={{color:"var(--a3)"}}>●</div><div className="stat-key">Live</div></div>
          </div>
        </div>
        <div className="sb-sec">
          <div className="sb-label">📋 Verbindungslog</div>
          <div className="log-box" ref={logRef} style={{height:100}}>
            {logs.map((l,i)=>(
              <div key={i} className="log-row">
                <span className="lt">{l.ts}</span>
                <span className={l.t==="ok"?"lo":l.t==="error"?"le":l.t==="warn"?"lw":"li"}>{l.m}</span>
              </div>
            ))}
          </div>
        </div>
        <div className="sb-sec">
          <div className="sb-label">💾 Gespeicherte Server</div>
          <div className="srv-list">
            {SAVED.map(s=>(
              <div key={s.id} className="srv-item" onClick={()=>connectSaved(s)}>
                <div>
                  <div className="srv-item-name">{s.emoji} {s.name}</div>
                  <div className="srv-item-url">{s.host}</div>
                  <div className="srv-item-badges">
                    <span className={`badge ${s.status==="online"?"b-green":"b-red"}`}>{s.status}</span>
                    <span className="badge b-blue">{s.type}</span>
                  </div>
                </div>
                <span style={{color:"var(--muted)"}}>›</span>
              </div>
            ))}
          </div>
        </div>
      </aside>
      <div className="content">
        <div className="content-hdr">
          <div>
            <div className="ch-title">Kanäle</div>
            <div className="ch-sub">{filteredCh.length} von {CHANNELS.length} Kanälen</div>
          </div>
          <input className="search" placeholder="🔍 Kanal suchen…" value={search} onChange={e=>setSearch(e.target.value)}/>
        </div>
        <div className="tabs">
          {CATS.map(c=><button key={c} className={`tab ${cat===c?"act":""}`} onClick={()=>setCat(c)}>{c}</button>)}
        </div>
        <div className="ch-area">
          {filteredCh.length===0?(
            <div className="empty"><div className="empty-ico">🔍</div><div className="empty-t">Keine Kanäle</div><div className="empty-s">Keine Treffer für diese Suche.</div></div>
          ):(
            <div className="ch-grid">
              {filteredCh.map(ch=>(
                <div key={ch.id} className={`ch-card ${playing?.id===ch.id?"live":""}`} onClick={()=>{setPlaying(ch);setPaused(false);}}>
                  <div className="ch-logo" style={{background:ch.color+"22",border:`1px solid ${ch.color}44`}}>{ch.emoji}</div>
                  <div className="ch-name">{ch.name}</div>
                  <div className="ch-group">{ch.group}</div>
                  <span className={`badge ${ch.quality==="4K"?"b-green":ch.quality==="FHD"?"b-blue":"b-grey"}`}>{ch.quality}</span>
                  {playing?.id===ch.id&&!paused&&<div className="live-bar"/>}
                </div>
              ))}
            </div>
          )}
        </div>
        {playing&&(
          <div className="player">
            <div className="pl-ch">
              <div className="pl-logo" style={{background:playing.color+"22",border:`1px solid ${playing.color}44`}}>{playing.emoji}</div>
              <div>
                <div className="pl-name">{playing.name}</div>
                <div className="pl-live"><div className="dot on" style={{width:6,height:6}}/>{paused?"Pausiert":"Live"}</div>
              </div>
            </div>
            <div className="pl-ctrls">
              <button className="ctrl" onClick={()=>{const i=CHANNELS.indexOf(playing);setPlaying(CHANNELS[(i-1+CHANNELS.length)%CHANNELS.length]);}}>⏮</button>
              <button className={`ctrl ${!paused?"act":""}`} onClick={()=>setPaused(p=>!p)}>{paused?"▶":"⏸"}</button>
              <button className="ctrl" onClick={()=>{const i=CHANNELS.indexOf(playing);setPlaying(CHANNELS[(i+1)%CHANNELS.length]);}}>⏭</button>
              <button className="ctrl" onClick={()=>setPlaying(null)}>⏹</button>
            </div>
            <div className="pl-right">
              <div className="sig">{[10,16,22,16,20].map((h,i)=><span key={i} style={{height:h}}/>)}</div>
              <div className="q-badge">{playing.quality}</div>
            </div>
          </div>
        )}
      </div>
    </div>
  )}
</>
```

);
}
