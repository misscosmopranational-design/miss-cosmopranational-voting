
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#050403">
<title>MISS COSMOPRANATIONAL | Official Voting</title>

<style>
:root {
 --bg:#050403;
 --panel:#15110a;
 --gold:#d6ad45;
 --line:#5b451c;
}
* {box-sizing:border-box}
body {
 margin:0;
 background:radial-gradient(ellipse at 50% 30%,#211806 0,#050403 58%);
 color:#f7f4eb;
 font-family:Arial,Helvetica,sans-serif;
}
header {
 min-height:82px;
 border-bottom:1px solid var(--line);
 display:flex;
 align-items:center;
 justify-content:space-between;
 padding:10px max(4vw,18px);
 background:#050403;
 position:sticky;
 top:0;
 z-index:100;
}
.brand {
 font-weight:900;
 letter-spacing:2px;
 color:var(--gold);
 font-size:clamp(15px,3vw,25px);
}
.brand small {
 display:block;
 color:#d8cba8;
 font-size:9px;
 letter-spacing:3px;
 margin-top:4px;
}
button {
 cursor:pointer;
 font-weight:700;
 border:0;
 border-radius:8px;
 padding:11px 14px;
 background:var(--gold);
 color:#171006;
}
button:hover {filter:brightness(1.12)}
button:disabled {opacity:.4;cursor:not-allowed}
.ghost {
 background:transparent;
 color:white;
 border:1px solid #80601f;
}
.danger {background:#9e333b;color:white}
.menu-btn {
 background:#1b1408;
 color:var(--gold);
 border:1px solid #80601f;
 border-radius:12px;
 width:55px;
 height:50px;
 font-size:27px;
 display:grid;
 place-items:center;
}
.menu {
 display:none;
 position:absolute;
 right:18px;
 top:75px;
 width:220px;
 background:#171108;
 border:1px solid var(--line);
 padding:12px;
 border-radius:12px;
 box-shadow:0 12px 30px #000b;
}
.menu.show {display:grid;gap:9px}
.menu button {width:100%;text-align:left}
main {width:min(1120px,92vw);margin:26px auto 60px}
.hero {
 width:100%;
 height:clamp(180px,43vw,430px);
 background:linear-gradient(135deg,#211806,#050403 65%,#30220b);
 border:1px solid #80601f;
 display:flex;
 align-items:center;
 justify-content:center;
 text-align:center;
 overflow:hidden;
}
.hero img {width:100%;height:100%;object-fit:cover}
.hero-placeholder {padding:25px}
.hero-placeholder h2 {
 font-size:clamp(26px,5vw,52px);
 margin:0 0 10px;
 letter-spacing:2px;
 color:#f1d486;
}
.hero-placeholder p {color:#c5b98e;letter-spacing:2px}
.section-title {font-size:clamp(25px,4vw,38px);margin:36px 0 20px}
.round-card {
 border:1px solid #80601f;
 border-radius:24px;
 background:linear-gradient(115deg,#211805,#090806);
 padding:25px 28px;
 margin-bottom:34px;
 box-shadow:0 15px 45px #0008;
}
.round-top {
 display:flex;
 justify-content:space-between;
 gap:15px;
 align-items:flex-start;
}
.round-title {
 font-size:clamp(23px,4vw,34px);
 font-weight:800;
 margin:0;
 text-transform:uppercase;
}
.live {
 background:#ed3e4a;
 color:white;
 border-radius:30px;
 padding:10px 18px;
 font-weight:800;
 white-space:nowrap;
}
.round-desc {
 color:#b9b09a;
 font-size:clamp(15px,2.5vw,20px);
 line-height:1.5;
 margin:18px 0;
}
.timer-row {
 border-top:1px solid #69501e;
 margin-top:22px;
 padding-top:18px;
 display:flex;
 align-items:center;
 gap:9px;
 flex-wrap:wrap;
}
.timer-label {font-weight:700;color:#b9b09a;margin-right:auto}
.timebox {
 background:#2a2110;
 border:1px solid #705827;
 border-radius:12px;
 padding:9px 12px;
 text-align:center;
 min-width:58px;
}
.timebox b {display:block;font-size:23px}
.timebox small {color:#b5a477}
.vote-link {margin-left:auto;background:none;color:#f0d181;font-size:18px}
.leaderboard {
 background:radial-gradient(circle at 30% 20%,#241b0b,#090806 55%);
 border-radius:28px;
 padding:25px;
 border:1px solid #80601f;
}
.leader-head {
 display:flex;
 align-items:flex-start;
 justify-content:space-between;
 gap:15px;
 flex-wrap:wrap;
}
.leader-head h2 {margin:0;font-size:clamp(26px,4vw,38px)}
.gold {color:var(--gold)}
.round-name {
 display:block;
 text-transform:uppercase;
 max-width:300px;
 line-height:1.2;
 color:var(--gold);
}
.rank-list {display:grid;gap:18px;margin-top:28px}
.rank-card {
 display:grid;
 grid-template-columns:minmax(120px,215px) 1fr;
 gap:24px;
 align-items:center;
 padding:20px;
 border:1px solid #57421c;
 border-radius:25px;
 background:linear-gradient(110deg,#1b1509,#0b0906);
 min-height:245px;
}
.rank-card.first {border-color:#a98737;background:linear-gradient(110deg,#2a200c,#100c06)}
.rank-card img {
 width:100%;
 height:210px;
 object-fit:cover;
 border-radius:18px;
 border:1px solid #9e8548;
 background:#18201d;
}
.rank-info {min-width:0}
.medal {font-size:30px;color:var(--gold)}
.rank-code {color:#aeb09e;margin-top:12px}
.rank-name {
 font-size:clamp(20px,3vw,27px);
 font-weight:800;
 margin:4px 0;
 text-transform:uppercase;
 overflow-wrap:anywhere;
}
.rank-country {color:#bdc8c3}
.percentage {font-size:clamp(30px,5vw,44px);font-weight:800;color:#f0d181;margin-top:10px}
.vote-count {color:#cfc3a2;font-size:13px;margin:3px 0 12px}
.vote-controls {
 margin-top:12px;
 padding:12px;
 border:1px solid #57421c;
 border-radius:12px;
 background:#0c0905;
}
.vote-controls strong {display:block;color:#e9d394;margin-bottom:9px;font-size:13px}
.vote-options {
 display:grid;
 grid-template-columns:repeat(5,minmax(0,1fr));
 gap:6px;
}
.vote-options button {padding:9px 4px;font-size:13px;border-radius:7px}
.vote-options button.chosen {
 outline:2px solid #fff1c1;
 background:#f3d98f;
}
.custom-row {display:flex;gap:7px;margin-top:8px}
.custom-row input {max-width:110px}
.remaining {font-size:12px;color:#c9b98b;margin-top:8px}
#allRanking {display:none}
.admin {display:none}
.admin-box {
 background:#100d08;
 border:1px solid var(--line);
 padding:22px;
 border-radius:18px;
 margin:18px 0;
}
.admin h2,.admin h3 {color:var(--gold)}
label {display:block;color:#d5c59e;font-size:14px;margin:12px 0 5px}
input,select,textarea {
 width:100%;
 padding:12px;
 border-radius:8px;
 border:1px solid #705827;
 background:#090704;
 color:white;
}
input[type=file] {padding:9px}
.formgrid {
 display:grid;
 grid-template-columns:repeat(auto-fit,minmax(210px,1fr));
 gap:12px;
}
.admin-delegate {
 display:flex;
 gap:12px;
 align-items:center;
 border-bottom:1px solid #55421e;
 padding:12px 0;
}
.admin-delegate img {width:62px;height:72px;object-fit:cover;border-radius:8px}
.admin-delegate div {flex:1}
.small {color:#9baaa3;font-size:12px;line-height:1.5}
.empty {
 color:#aab9b2;
 padding:25px;
 text-align:center;
 border:1px dashed #705827;
 border-radius:12px;
}
.round-admin {
 padding:14px;
 border:1px solid #59451f;
 border-radius:12px;
 margin:10px 0;
 background:#171108;
}
.round-admin.active-round {border-color:#d6ad45}
.round-admin-head {
 display:flex;
 justify-content:space-between;
 gap:10px;
 align-items:center;
 flex-wrap:wrap;
}
.notice {
 border:1px solid #80601f;
 background:#211805;
 color:#e9d394;
 padding:12px;
 border-radius:10px;
 font-size:13px;
 line-height:1.5;
}
footer {
 text-align:center;
 color:#a08b5b;
 padding:30px;
 border-top:1px solid #5b451c;
}
@media(max-width:600px) {
 header {height:76px}
 .menu {right:12px;top:68px}
 .round-card {padding:20px 17px}
 .rank-card {grid-template-columns:105px 1fr;gap:12px;padding:11px;min-height:150px}
 .rank-card img {height:150px}
 .leaderboard {padding:16px}
 .timer-label {width:100%}
 .vote-options {grid-template-columns:repeat(5,minmax(0,1fr))}
 .vote-options button {font-size:11px;padding:8px 2px}
}
</style>
</head>

<body>
<header>
 <div class="brand">
  MISS COSMOPRANATIONAL
  <small>OFFICIAL ONLINE VOTING</small>
 </div>

 <button class="menu-btn" id="menuButton" aria-label="Open menu"
 aria-expanded="false" type="button">☰</button>

 <nav class="menu" id="menu">
  <button class="ghost" type="button" onclick="goHome()">Voting Home</button>
  <button class="ghost" type="button" onclick="adminLogin()">Admin Login</button>
 </nav>
</header>

<main>
 <section class="hero" id="hero">
  <div class="hero-placeholder">
   <h2>MISS COSMOPRANATIONAL</h2>
   <p>OFFICIAL ONLINE VOTING</p>
  </div>
 </section>

 <section id="publicPage">
  <h2 class="section-title">Official Voting</h2>

  <div class="round-card">
   <div class="round-top">
    <h2 class="round-title" id="roundTitle">MOST POPULAR VOTE</h2>
    <span class="live" id="liveBadge">CLOSED</span>
   </div>

   <p class="round-desc" id="roundDescription">Support your favorite delegate.</p>

   <div class="timer-row">
    <span class="timer-label" id="timerLabel">VOTING CLOSED</span>
    <div class="timebox"><b id="days">00</b><small>DAYS</small></div>
    <div class="timebox"><b id="hours">00</b><small>HOURS</small></div>
    <div class="timebox"><b id="minutes">00</b><small>MIN</small></div>
    <div class="timebox"><b id="seconds">00</b><small>SEC</small></div>
    <button class="vote-link" type="button" onclick="document.getElementById('leaderboard').scrollIntoView({behavior:'smooth'})">VOTE NOW ❯❯</button>
   </div>

   <p class="small" id="multiplierText">Vote multiplier: 1x</p>
  </div>

  <section class="leaderboard" id="leaderboard">
   <div class="leader-head">
    <h2>Leaderboard <span class="gold">—</span>
     <span class="round-name" id="leaderTitle">MOST POPULAR VOTE</span>
    </h2>
    <button class="ghost" type="button" onclick="toggleAll()">VIEW ALL RANKING ❯❯</button>
   </div>
   <div class="rank-list" id="topRanking"></div>
   <div class="rank-list" id="allRanking"></div>
  </section>
 </section>

 <section class="admin" id="admin">

  <div class="admin-box">
   <h2>ADMIN DASHBOARD</h2>
   <p>Manage voting rounds, delegates, schedules, banner, and results.</p>
   <button class="ghost" type="button" onclick="logout()">Log Out</button>
  </div>

  <div class="admin-box">
   <h3>Create / Edit Voting Round</h3>
   <input type="hidden" id="editingRoundId">

   <label>Voting Round / Category Name</label>
   <input id="aTitle" placeholder="e.g. BEST IN EVENING GOWN">

   <label>Description</label>
   <textarea id="aDesc" rows="2" placeholder="Describe this voting category"></textarea>

   <div class="formgrid">
    <div><label>Voting Start</label><input type="datetime-local" id="aStart"></div>
    <div><label>Voting End</label><input type="datetime-local" id="aEnd"></div>
   </div>

   <div class="formgrid">
    <div>
     <label>Vote Multiplier</label>
     <select id="aMultiplier">
      <option value="1">1x - Normal</option>
      <option value="2">2x - Double votes</option>
      <option value="3">3x - Triple votes</option>
     </select>
    </div>
    <div>
     <label>Maximum votes per voter, per delegate</label>
     <input id="aMaxVotes" type="number" min="10" max="100" step="10" value="100">
    </div>
   </div>

   <div class="formgrid">
    <button type="button" onclick="saveRound()">Save Voting Round</button>
    <button class="ghost" type="button" onclick="clearRoundForm()">Clear / New Round</button>
   </div>
   <p class="small">Each voting round has its own schedule, multiplier, delegate list, and leaderboard.</p>
  </div>

  <div class="admin-box">
   <h3>Manage Voting Rounds</h3>
   <div id="roundAdminList"></div>
  </div>

  <div class="admin-box">
   <h3>Delegate Management</h3>
   <p class="small">Add delegates to the currently selected voting round.</p>

   <label>Select Voting Round</label>
   <select id="delegateRoundSelect"></select>

   <label>Delegate Name</label>
   <input id="dName" placeholder="Delegate name">

   <label>Country</label>
   <input id="dCountry" placeholder="Country">

   <label>Delegate Photo — choose from your phone gallery</label>
   <input type="file" id="dPhoto" accept="image/*">

   <button type="button" onclick="addDelegate()">ADD DELEGATE</button>
   <div id="delegateAdminList"></div>
  </div>

  <div class="admin-box">
   <h3>Event Banner</h3>
   <label>Choose banner image from your phone</label>
   <input type="file" id="bannerFile" accept="image/*">
   <button type="button" onclick="saveBanner()">Upload Banner</button>
   <button class="ghost" type="button" onclick="removeBanner()">Remove Banner</button>
  </div>

  <div class="admin-box">
   <h3>Voting Results</h3>
   <div id="adminResults"></div>
   <button class="danger" type="button" onclick="resetCurrentVotes()">Reset Votes for Selected Round</button>
  </div>

  <div class="admin-box">
   <h3>Important Security Note</h3>
   <div class="notice">
    This browser-only version stores information on this device.
    It is not yet a shared official voting system. A cloud database,
    secure admin authentication and server-side vote validation are
    required before publishing it for public voting.
   </div>
  </div>
 </section>
</main>

<footer>MISS COSMOPRANATIONAL • OFFICIAL VOTING PLATFORM</footer>

<script>
"use strict";

const KEY = "mcp_grandvote_multi_round_v3";
const VOTER_KEY = "mcp_voter_usage_v3";

const DEFAULT_ROUND = {
 id:"round_"+Date.now(),
 title:"MOST POPULAR VOTE",
 description:"Support your favorite delegate.",
 start:"",
 end:"",
 multiplier:1,
 maxVotes:100,
 active:false,
 delegates:[],
 votes:{}
};

function readDB() {
 try {
  const saved = JSON.parse(localStorage.getItem(KEY) || "null");
  if (saved && Array.isArray(saved.rounds)) {
   return {rounds:saved.rounds,banner:saved.banner || ""};
  }
 } catch(e) {}
 return {rounds:[{...DEFAULT_ROUND}] ,banner:""};
}

let db = readDB();
let selectedRoundId = db.rounds[0]?.id || null;
let chosenAmounts = {};
let showAll = false;
let timerInterval = null;
let isAdmin = false;

const $ = id => document.getElementById(id);

function persist() {
 try {
  localStorage.setItem(KEY,JSON.stringify(db));
 } catch(e) {
  alert("Browser storage is full. Please use smaller photos.");
 }
}

function readUsage() {
 try {return JSON.parse(localStorage.getItem(VOTER_KEY) || "{}");}
 catch(e) {return {};}
}

function saveUsage(data) {
 localStorage.setItem(VOTER_KEY,JSON.stringify(data));
}

function currentRound() {
 return db.rounds.find(r=>r.id===selectedRoundId) || db.rounds[0] || null;
}

function roundUsageKey(rid,did) {
 return rid+"::"+did;
}

function usedVotes(rid,did) {
 return Number(readUsage()[roundUsageKey(rid,did)] || 0);
}

/* FIXED MENU: click, outside click and Escape */
function toggleMenu(force) {
 const menu = $("menu");
 const button = $("menuButton");
 const shouldOpen = typeof force === "boolean"
  ? force
  : !menu.classList.contains("show");

 menu.classList.toggle("show",shouldOpen);
 button.setAttribute("aria-expanded",String(shouldOpen));
}

$("menuButton").addEventListener("click",function(e) {
 e.stopPropagation();
 toggleMenu();
});

$("menu").addEventListener("click",function(e) {
 e.stopPropagation();
});

document.addEventListener("click",function() {
 toggleMenu(false);
});

document.addEventListener("keydown",function(e) {
 if(e.key==="Escape") toggleMenu(false);
});

function goHome() {
 $("admin").style.display="none";
 $("publicPage").style.display="block";
 toggleMenu(false);
 render();
 window.scrollTo({top:0,behavior:"smooth"});
}

function adminLogin() {
 toggleMenu(false);
 const username = prompt("Admin username:");
 if(username===null) return;

 const password = prompt("Admin password:");
 if(password===null) return;

 /* DEMO ONLY: replace with secure cloud authentication */
 if(username==="MCPFOUNDER" && password==="MCP2026") {
  isAdmin=true;
  $("publicPage").style.display="none";
  $("admin").style.display="block";
  renderAdmin();
  window.scrollTo({top:0,behavior:"smooth"});
 } else {
  alert("Incorrect login.");
 }
}

function logout() {
 isAdmin=false;
 goHome();
}

function openNow(r=currentRound()) {
 if(!r || !r.active || !r.start || !r.end) return false;

 const now=Date.now();
 const start=new Date(r.start).getTime();
 const end=new Date(r.end).getTime();

 if(now>=end) {
  r.active=false;
  persist();
  return false;
 }
 return now>=start && now<end;
}

function roundStatus(r) {
 if(!r.active) return "CLOSED";
 const now=Date.now();

 if(r.end && now>=new Date(r.end).getTime()) {
  r.active=false;
  persist();
  return "CLOSED";
 }
 if(r.start && now<new Date(r.start).getTime()) return "UPCOMING";
 return openNow(r) ? "LIVE" : "CLOSED";
}

function clearRoundForm() {
 ["editingRoundId","aTitle","aDesc","aStart","aEnd"].forEach(id=>$(id).value="");
 $("aMultiplier").value="1";
 $("aMaxVotes").value="100";
}

function saveRound() {
 if(!isAdmin) return alert("Admin access required.");

 const id=$("editingRoundId").value;
 const title=$("aTitle").value.trim();
 const start=$("aStart").value;
 const end=$("aEnd").value;
 const max=Number($("aMaxVotes").value);

 if(!title) return alert("Enter a voting category name.");

 if(start && end && new Date(end)<=new Date(start))
  return alert("End time must be later than start time.");

 if(!Number.isInteger(max) || max<10 || max>100)
  return alert("Maximum votes must be from 10 to 100.");

 if(id) {
  const r=db.rounds.find(x=>x.id===id);
  if(!r) return;
  Object.assign(r,{
   title,
   description:$("aDesc").value.trim(),
   start,end,
   multiplier:Number($("aMultiplier").value),
   maxVotes:max
  });
 } else {
  const r={
   id:"round_"+Date.now()+"_"+Math.random().toString(16).slice(2),
   title,
   description:$("aDesc").value.trim(),
   start,end,
   multiplier:Number($("aMultiplier").value),
   maxVotes:max,
   active:false,
   delegates:[],
   votes:{}
  };
  db.rounds.push(r);
  selectedRoundId=r.id;
 }

 persist();
 clearRoundForm();
 render();
 renderAdmin();
 alert("Voting round saved.");
}

function editRound(id) {
 if(!isAdmin) return;
 const r=db.rounds.find(x=>x.id===id);
 if(!r) return;

 $("editingRoundId").value=r.id;
 $("aTitle").value=r.title;
 $("aDesc").value=r.description || "";
 $("aStart").value=r.start || "";
 $("aEnd").value=r.end || "";
 $("aMultiplier").value=r.multiplier || 1;
 $("aMaxVotes").value=r.maxVotes || 100;

 window.scrollTo({
  top:$("admin").offsetTop,
  behavior:"smooth"
 });
}

function selectRound(id) {
 selectedRoundId=id;
 showAll=false;
 render();
 renderAdmin();
}

function activateRound(id) {
 if(!isAdmin) return;
 const r=db.rounds.find(x=>x.id===id);
 if(!r) return;

 if(!r.start || !r.end || new Date(r.end)<=new Date(r.start))
  return alert("Set a valid start and end time first.");

 if(Date.now()>=new Date(r.end).getTime())
  return alert("End time has passed. Set a new schedule.");

 r.active=true;
 persist();
 render();
 renderAdmin();
}

function closeRound(id) {
 if(!isAdmin) return;
 const r=db.rounds.find(x=>x.id===id);
 if(!r) return;
 r.active=false;
 persist();
 render();
 renderAdmin();
}

function deleteRound(id) {
 if(!isAdmin) return;
 if(db.rounds.length===1)
  return alert("You must keep at least one voting round.");

 if(!confirm("Delete this voting round and all its results?")) return;

 db.rounds=db.rounds.filter(x=>x.id!==id);
 selectedRoundId=db.rounds[0].id;
 persist();
 render();
 renderAdmin();
}

function compress(file,callback) {
 if(!file || !file.type.startsWith("image/"))
  return alert("Please choose an image.");

 const reader=new FileReader();
 reader.onload=()=>{
  const im=new Image();
  im.onload=()=>{
   const canvas=document.createElement("canvas");
   const scale=Math.min(1,1000/Math.max(im.width,im.height));
   canvas.width=im.width*scale;
   canvas.height=im.height*scale;
   canvas.getContext("2d").drawImage(im,0,0,canvas.width,canvas.height);
   callback(canvas.toDataURL("image/jpeg",.72));
  };
  im.onerror=()=>alert("Unable to read this image.");
  im.src=reader.result;
 };
 reader.onerror=()=>alert("Unable to load this file.");
 reader.readAsDataURL(file);
}

function addDelegate() {
 if(!isAdmin) return;
 const r=db.rounds.find(x=>x.id===$("delegateRoundSelect").value);
 if(!r) return alert("Create or select a voting round first.");

 const name=$("dName").value.trim();
 const country=$("dCountry").value.trim();
 const file=$("dPhoto").files[0];

 if(!name || !country || !file)
  return alert("Enter name, country, and choose a photo.");

 compress(file,url=>{
  r.delegates.push({
   id:Date.now().toString()+Math.random().toString(16).slice(2),
   name,country,photo:url
  });
  persist();
  $("dName"
