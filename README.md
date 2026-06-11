<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ClearBid QuickQuote — Glass & Glazing Estimates in Minutes</title>
<style>
:root{--navy:#0F2A43;--teal:#0E7C7B;--teal-dark:#0A5E5D;--light:#EBF4F4;--ink:#1A1A1A;--gray:#5A6B7A;--red:#D94F4F;--border:#C9D6D6}
*{margin:0;padding:0;box-sizing:border-box}
body{font-family:'Segoe UI',system-ui,Arial,sans-serif;background:#F4F7F9;color:var(--ink);line-height:1.5}
.wrap{max-width:1080px;margin:0 auto;padding:0 16px}
header{background:var(--navy);color:#fff;padding:14px 0}
header .wrap{display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:8px}
.logo{font-weight:800;font-size:1.2rem;letter-spacing:.5px}
.logo span{color:#5BC8C7}
.tagline{font-size:.8rem;color:#8FB0C4}
h2{color:var(--navy);font-size:1.15rem;margin-bottom:12px;border-left:4px solid var(--teal);padding-left:10px}
.panel{background:#fff;border:1px solid var(--border);border-radius:10px;padding:20px;margin:18px 0}
label{display:block;font-size:.8rem;font-weight:600;color:var(--gray);margin-bottom:3px}
input,select,textarea{width:100%;padding:8px 10px;border:1px solid var(--border);border-radius:6px;font-size:.92rem;font-family:inherit;background:#fff}
input:focus,select:focus,textarea:focus{outline:2px solid var(--teal);border-color:var(--teal)}
.grid{display:grid;gap:12px}
.g2{grid-template-columns:1fr 1fr}.g3{grid-template-columns:1fr 1fr 1fr}.g4{grid-template-columns:2fr 1fr 1fr 1fr}
@media(max-width:680px){.g2,.g3,.g4{grid-template-columns:1fr}}
button{cursor:pointer;border:none;border-radius:6px;font-weight:700;font-size:.92rem;padding:10px 18px;font-family:inherit}
.btn-primary{background:var(--teal);color:#fff}.btn-primary:hover{background:var(--teal-dark)}
.btn-navy{background:var(--navy);color:#fff}
.btn-ghost{background:transparent;color:var(--red);border:1px solid var(--red);padding:6px 12px;font-size:.8rem}
.btn-add{background:var(--light);color:var(--teal-dark);border:1.5px dashed var(--teal);width:100%;padding:12px}
table{width:100%;border-collapse:collapse;font-size:.9rem}
th{background:var(--navy);color:#fff;text-align:left;padding:8px 10px;font-size:.8rem}
td{padding:8px 10px;border-bottom:1px solid var(--border)}
tr:nth-child(even) td{background:var(--light)}
.right{text-align:right}
.item-card{border:1px solid var(--border);border-radius:8px;padding:14px;margin-bottom:12px;background:#FAFCFC}
.item-head{display:flex;justify-content:space-between;align-items:center;margin-bottom:10px;gap:8px;flex-wrap:wrap}
.item-title{font-weight:700;color:var(--navy)}
.totals{font-size:1rem}
.totals .row{display:flex;justify-content:space-between;padding:6px 0;border-bottom:1px solid var(--border)}
.totals .grand{font-size:1.4rem;font-weight:800;color:var(--teal-dark);border-bottom:none;padding-top:12px}
.hint{font-size:.78rem;color:var(--gray);margin-top:3px}
.warn{background:#FDF3E7;border:1px solid #E8B96A;border-radius:6px;padding:8px 12px;font-size:.82rem;margin-top:10px;display:none}
.ok{background:#EAF7EF;border-color:#7BC894}
.actionbar{display:flex;gap:10px;flex-wrap:wrap;margin:20px 0 40px}
.muted{color:var(--gray);font-size:.82rem}
footer{padding:24px 0 40px;text-align:center;color:var(--gray);font-size:.8rem}
#proposal{display:none}
.prop-page{background:#fff;max-width:820px;margin:20px auto;padding:48px 56px;border:1px solid var(--border)}
.prop-header{display:flex;justify-content:space-between;align-items:flex-start;border-bottom:3px solid var(--teal);padding-bottom:14px;margin-bottom:18px;gap:12px}
.prop-co{font-size:1.5rem;font-weight:800;color:var(--navy)}
.prop-co-sub{font-size:.85rem;color:var(--teal-dark)}
.prop-contact{font-size:.8rem;text-align:right;color:var(--gray)}
.prop-meta{display:flex;justify-content:space-between;flex-wrap:wrap;gap:6px;font-size:.88rem;margin-bottom:16px}
.prop-sec{font-weight:800;color:var(--teal-dark);font-size:.95rem;margin:18px 0 6px;letter-spacing:.5px}
.prop-body{font-size:.9rem}
.prop-table th{font-size:.78rem}
.prop-foot{margin-top:28px;border-top:1px solid var(--border);padding-top:12px;font-size:.78rem;color:var(--gray);text-align:center}
.sig-row{display:flex;gap:40px;margin-top:30px;font-size:.85rem}
.sig{flex:1;border-top:1px solid var(--ink);padding-top:4px}
@media print{
  body{background:#fff}
  header,#builder,.actionbar,footer,.no-print{display:none !important}
  #proposal{display:block !important}
  .prop-page{border:none;margin:0;padding:0;max-width:none}
}
</style>
</head>
<body>

<header>
  <div class="wrap">
    <div>
      <div class="logo">CLEAR<span>BID</span> QUICKQUOTE</div>
      <div class="tagline">Bid-ready glass &amp; glazing proposals in minutes</div>
    </div>
    <div class="muted" style="color:#8FB0C4">All data stays in your browser — nothing is uploaded.</div>
  </div>
</header>

<div class="wrap" id="builder">

  <div class="panel">
    <h2>1 · Your Shop (saved on this device)</h2>
    <div class="grid g2">
      <div><label>Company name</label><input id="coName" placeholder="Lone Star Glass & Glazing" onchange="saveShop()"></div>
      <div><label>Tagline / license line</label><input id="coTag" placeholder="Commercial Glass & Glazing | TX License #..." onchange="saveShop()"></div>
      <div><label>Phone</label><input id="coPhone" placeholder="(xxx) xxx-xxxx" onchange="saveShop()"></div>
      <div><label>Email</label><input id="coEmail" placeholder="bids@yourshop.com" onchange="saveShop()"></div>
    </div>
  </div>

  <div class="panel">
    <h2>2 · Project</h2>
    <div class="grid g2">
      <div><label>Project name</label><input id="pjName" placeholder="Retail Storefront — Suite 100"></div>
      <div><label>Client / GC</label><input id="pjClient" placeholder="ABC Commercial Builders"></div>
      <div><label>Project address</label><input id="pjAddr" placeholder="4521 Main St, City, TX"></div>
      <div><label>Proposal number</label><input id="pjNum" placeholder="Auto" ></div>
      <div>
        <label>Floor level (affects labor rates)</label>
        <select id="pjLevel" onchange="recalc()">
          <option value="0">Ground floor</option>
          <option value="1">Elevated (2–4 stories)</option>
          <option value="2">High-rise (5+ stories)</option>
        </select>
      </div>
      <div>
        <label>Overhead &amp; profit markup %</label>
        <input id="pjMarkup" type="number" value="22" min="0" max="60" onchange="recalc()">
        <div class="hint">Guide: &lt;$10k → 25–30% · $10–50k → 20–25% · $50–150k → 18–22% · larger → 15–20%</div>
      </div>
    </div>
  </div>

  <div class="panel">
    <h2>3 · Scope Items</h2>
    <div id="items"></div>
    <button class="btn-add" onclick="addItem()">+ Add scope item</button>
    <div class="hint" style="margin-top:8px">Rates are editable market defaults (DFW commercial, mid-range). Always review against your local costs.</div>
  </div>

  <div class="panel">
    <h2>4 · Totals</h2>
    <div class="totals" id="totals"></div>
    <div class="warn" id="sanity"></div>
  </div>

  <div class="actionbar">
    <button class="btn-primary" onclick="buildProposal();window.print()">⬇ Generate Proposal (PDF)</button>
    <button class="btn-navy" onclick="buildProposal();document.getElementById('proposal').style.display='block';document.getElementById('proposal').scrollIntoView({behavior:'smooth'})">Preview Proposal</button>
  </div>
</div>

<div id="proposal"></div>

<footer>ClearBid QuickQuote · Estimates are budgetary tools — verify quantities and pricing before submitting any bid. Not a substitute for engineering or professional review.</footer>

<script>
const GLASS = {
  "Clear tempered 1/4\" (single)":10, "Clear IGU 1\"":18, "Low-E IGU 1\"":23,
  "Tinted IGU (bronze/gray)":22, "Spandrel":26, "Laminated safety 1/2\"":28,
  "Tempered laminated":35, "Low-E high-performance":32, "Smart Glass / PDLC":85,
  "Electrochromic smart glass":115
};
const FINISH = {"Clear anodized":0,"Dark bronze anodized":2.5,"Black anodized":2.5,"Kynar painted":5,"Custom RAL Kynar":7.5};
const SYSTEMS = {
  "Storefront — standard":      {frame:16, labor:[16,21,28], unit:"SF"},
  "Storefront — heavy duty":    {frame:21, labor:[16,21,28], unit:"SF"},
  "Curtain wall — stick built": {frame:30, labor:[21,27,36], unit:"SF"},
  "Curtain wall — unitized":    {frame:48, labor:[17,24,33], unit:"SF"},
  "Commercial windows (punched)":{frame:19, labor:[12.5,17.5,24], unit:"SF"},
  "Skylight / overhead glazing":{frame:38, labor:[26,33,0], unit:"SF"},
  "Glass replacement (existing frame)":{frame:0, labor:[10,15,21.5], unit:"SF"},
  "Smart Glass installation":   {frame:16, labor:[19,26,35], unit:"SF"}
};
const DOORS = {
  "Single aluminum door":1800, "Single door — heavy duty / ADA":2400,
  "Double door set":3600, "Double door — heavy duty / ADA":4800,
  "All-glass frameless door":3200, "Automatic sliding door":8500,
  "Automatic sliding — heavy traffic":12000, "Storefront sidelite":850, "Transom":600
};
const RAILS = {
  "Frameless — channel base":240, "Frameless — point fitting":290,
  "Post & panel — aluminum":185, "Post & panel — stainless":250
};
const SEALANT_SF = 2.0, FREIGHT = 600, DEBRIS = 350;

let items = [];
let nextId = 1;

function saveShop(){
  const s = {n:el('coName').value, t:el('coTag').value, p:el('coPhone').value, e:el('coEmail').value};
  try{ localStorage.setItem('cb_shop', JSON.stringify(s)); }catch(e){}
}
function loadShop(){
  try{
    const s = JSON.parse(localStorage.getItem('cb_shop')||'null');
    if(s){ el('coName').value=s.n||''; el('coTag').value=s.t||''; el('coPhone').value=s.p||''; el('coEmail').value=s.e||''; }
  }catch(e){}
}
function el(id){return document.getElementById(id)}
function money(n){return '$'+Math.round(n).toLocaleString('en-US')}

function addItem(kind){
  items.push({id:nextId++, kind:'glazing', system:Object.keys(SYSTEMS)[0], glass:Object.keys(GLASS)[2],
              finish:Object.keys(FINISH)[0], qty:0, door:Object.keys(DOORS)[3], rail:Object.keys(RAILS)[0],
              ovGlass:null, ovFrame:null, ovLabor:null, ovUnit:null});
  render();
}
function delItem(id){ items = items.filter(i=>i.id!==id); render(); }
function upd(id, field, val){
  const it = items.find(i=>i.id===id); if(!it) return;
  if(['qty','ovGlass','ovFrame','ovLabor','ovUnit'].includes(field)) val = val===''?null:parseFloat(val);
  it[field]=val;
  if(field==='kind'){ it.ovGlass=it.ovFrame=it.ovLabor=it.ovUnit=null; render(); return; }
  if(['system','glass','finish','door','rail'].includes(field)){ render(); return; }
  recalc();
}
function rates(it){
  const lvl = parseInt(el('pjLevel').value);
  if(it.kind==='glazing'){
    const sys=SYSTEMS[it.system];
    const labor = sys.labor[lvl]||sys.labor[1];
    return {
      glass: it.ovGlass ?? GLASS[it.glass],
      frame: it.ovFrame ?? (sys.frame + (sys.frame>0?FINISH[it.finish]:0)),
      labor: it.ovLabor ?? labor
    };
  }
  if(it.kind==='door') return {unit: it.ovUnit ?? DOORS[it.door]};
  return {unit: it.ovUnit ?? RAILS[it.rail]};
}
function itemTotal(it){
  const r = rates(it), q = it.qty||0;
  if(it.kind==='glazing') return q*(r.glass+r.frame+r.labor);
  return q*r.unit;
}

function render(){
  const host = el('items'); host.innerHTML='';
  items.forEach(it=>{
    const r = rates(it);
    const card = document.createElement('div'); card.className='item-card';
    let inner = `<div class="item-head">
      <select style="max-width:240px" onchange="upd(${it.id},'kind',this.value)">
        <option value="glazing" ${it.kind==='glazing'?'selected':''}>Glazed system (by SF)</option>
        <option value="door" ${it.kind==='door'?'selected':''}>Door / entrance (each)</option>
        <option value="rail" ${it.kind==='rail'?'selected':''}>Glass railing (by LF)</option>
      </select>
      <span class="item-title" id="t${it.id}">${money(itemTotal(it))}</span>
      <button class="btn-ghost" onclick="delItem(${it.id})">Remove</button>
    </div>`;
    if(it.kind==='glazing'){
      inner += `<div class="grid g3">
        <div><label>System</label><select onchange="upd(${it.id},'system',this.
