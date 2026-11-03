<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>制限時間つき暗記カード</title>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Zen+Kaku+Gothic+New:wght@400;500;700&display=swap">
<style>
:root{--bg:#eef1f5;--panel:#fff;--ink:#1d2736;--sub:#5d6b80;--line:#d5dce6;--pri:#2c4a9a;--priink:#fff;--ok:#1b8a5a;--ng:#c8403f;--warn:#d98a00;--flag:#e0a100;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#121821;--panel:#1b2330;--ink:#e6ebf3;--sub:#9aa7bb;--line:#2f3a4b;--pri:#8fa8f0;--priink:#10192b;--ok:#4cc38a;--ng:#f07674;--warn:#f0b02e;--flag:#f0c030}}
:root[data-theme="dark"]{--bg:#121821;--panel:#1b2330;--ink:#e6ebf3;--sub:#9aa7bb;--line:#2f3a4b;--pri:#8fa8f0;--priink:#10192b;--ok:#4cc38a;--ng:#f07674;--warn:#f0b02e;--flag:#f0c030}
*{box-sizing:border-box}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);color:var(--ink);font:16px/1.7 "Zen Kaku Gothic New","Hiragino Sans","Yu Gothic",Meiryo,sans-serif}
body::before{content:"";position:fixed;inset:0 0 auto;height:env(safe-area-inset-top,0px);background:var(--bg);z-index:10}
main{max-width:640px;margin:0 auto;padding:12px 14px 48px}
h1{font-size:19px;margin:6px 0 10px;font-weight:700}
nav{display:flex;gap:4px;border-bottom:2px solid var(--line);margin-bottom:14px}
nav button{flex:1;background:none;border:0;padding:10px 4px;font:inherit;font-weight:500;color:var(--sub);border-bottom:3px solid transparent;margin-bottom:-2px;cursor:pointer}
nav button[aria-selected=true]{color:var(--pri);border-color:var(--pri);font-weight:700}
.panel{background:var(--panel);border:1px solid var(--line);border-radius:12px;padding:16px;margin-bottom:12px}
label{display:block;font-weight:500;margin:10px 0 4px}
input[type=text],input[type=number],textarea,select{width:100%;font:inherit;color:var(--ink);background:var(--bg);border:1px solid var(--line);border-radius:8px;padding:9px 10px}
textarea{min-height:68px;resize:vertical}
button{font:inherit;cursor:pointer}
button:focus-visible,input:focus-visible,textarea:focus-visible,select:focus-visible{outline:3px solid var(--pri);outline-offset:2px}
.btn{background:var(--pri);color:var(--priink);border:0;border-radius:10px;padding:11px 18px;font-weight:700}
.btn.alt{background:transparent;color:var(--pri);border:1.5px solid var(--pri)}
.btn.ok{background:var(--ok);color:#fff}.btn.ng{background:var(--ng);color:#fff}
.btn.sm{padding:5px 10px;font-size:14px;font-weight:500}
.row{display:flex;gap:10px;flex-wrap:wrap;align-items:center}
.row>.grow{flex:1}
.modes{display:grid;gap:6px}
.modes label{display:flex;gap:8px;align-items:center;margin:0;padding:9px 10px;border:1px solid var(--line);border-radius:8px;font-weight:400}
.modes label:has(input:checked){border-color:var(--pri);background:var(--bg)}
.modes span{margin-left:auto;color:var(--sub);font-size:14px}
.bar{height:10px;background:var(--line);border-radius:5px;overflow:hidden;margin:6px 0 4px}
.bar i{display:block;height:100%;width:100%;background:var(--pri)}
.bar.low i{background:var(--warn)}.bar.crit i{background:var(--ng)}
.meta{display:flex;justify-content:space-between;color:var(--sub);font-size:14px}
.q{font-size:22px;font-weight:700;line-height:1.5;margin:18px 0;white-space:pre-wrap;word-break:break-word;min-height:3em}
.a{font-size:19px;white-space:pre-wrap;word-break:break-word;padding:12px;border-left:4px solid var(--pri);background:var(--bg);border-radius:0 8px 8px 0;margin:8px 0 14px}
.flag{background:none;border:1.5px solid var(--line);color:var(--sub);border-radius:20px;padding:3px 12px;font-size:14px}
.flag[aria-pressed=true]{border-color:var(--flag);color:var(--flag);font-weight:700}
.big{font-size:44px;font-weight:700;line-height:1.2}
.item{border-top:1px solid var(--line);padding:10px 0}
.item:first-child{border-top:0}
.item b{display:block;white-space:pre-wrap;word-break:break-word}
.item small{color:var(--sub);white-space:pre-wrap;word-break:break-word}
.tag{font-size:12px;padding:1px 7px;border-radius:10px;border:1px solid currentColor;margin-right:4px}
.note{color:var(--sub);font-size:14px;margin:6px 0 0}
.msg{margin-top:10px;font-weight:500}
[hidden]{display:none!important}
@media (prefers-reduced-motion:no-preference){.bar i{transition:width .1s linear}}
</style>
</head>
<body>
<main>
<h1>制限時間つき暗記カード</h1>
<div class="row" style="margin-bottom:10px"><label for="deck" style="margin:0">問題集</label><select id="deck" class="grow"></select></div>
<nav role="tablist">
<button role="tab" data-tab="study" aria-selected="true">学習</button>
<button role="tab" data-tab="cards" aria-selected="false">問題</button>
<button role="tab" data-tab="io" aria-selected="false">入出力</button>
</nav>

<section id="study">
<div class="panel" id="setup">
<label>復習する範囲</label>
<div class="modes" id="modes">
<label><input type="radio" name="mode" value="all"> すべての問題<span id="nAll"></span></label>
<label><input type="radio" name="mode" value="flag"> チェックした問題だけ<span id="nFlag"></span></label>
<label><input type="radio" name="mode" value="wrong"> 不正解だった問題だけ<span id="nWrong"></span></label>
</div>
<label for="limit">1問あたりの制限時間</label>
<div class="row">
<select id="limit" class="grow"><option value="0">なし</option><option value="10">10秒</option><option value="20">20秒</option><option value="30">30秒</option><option value="60">60秒</option><option value="x">自分で決める</option></select>
<input type="number" id="custom" min="1" max="600" placeholder="秒" style="width:90px" hidden>
</div>
<p class="note">問題ごとに秒数を決めてある場合は、そちらを優先します。</p>
<label><input type="checkbox" id="shuffle"> 順番をシャッフルする</label>
<div class="row" style="margin-top:14px"><button class="btn" id="start">学習をはじめる</button></div>
<p class="msg" id="setupMsg"></p>
</div>

<div class="panel" id="play" hidden>
<div class="meta"><span id="prog"></span><span id="left"></span></div>
<div class="bar" id="bar"><i></i></div>
<div class="row" style="justify-content:space-between"><button class="flag" id="flagBtn" aria-pressed="false">☆ チェック</button><button class="btn alt sm" id="quit">やめる</button></div>
<div class="q" id="qText"></div>
<div id="ans" hidden><div class="a" id="aText"></div><p class="msg" id="tmsg" hidden></p></div>
<div class="row" id="ctrl">
<button class="btn grow" id="reveal">答えを見る</button>
</div>
<div class="row" id="judge" hidden>
<button class="btn ok grow" id="okBtn">正解</button><button class="btn ng grow" id="ngBtn">不正解</button>
</div>
<div class="row" id="nextRow" hidden><button class="btn grow" id="nextBtn">次へ</button></div>
</div>

<div class="panel" id="result" hidden>
<div class="meta"><span>結果</span></div>
<div class="big"><span id="rOk" style="color:var(--ok)"></span> / <span id="rAll"></span></div>
<p id="rText"></p>
<div class="row">
<button class="btn" id="retryWrong">不正解だけ復習</button>
<button class="btn alt" id="again">もう一度</button>
<button class="btn alt" id="back">戻る</button>
</div>
</div>
</section>

<section id="cards" hidden>
<div class="panel"><label for="dname">問題集の名前（教科ごとなどに分けられます）</label><input type="text" id="dname"><div class="row" style="margin-top:10px"><button class="btn alt sm" id="dNew">新しい問題集を作る</button><button class="btn alt sm" id="dRen">名前を変える</button><button class="btn alt sm" id="dDel">この問題集を削除</button></div><p class="msg" id="dMsg"></p></div>
<div class="panel">
<label for="fq">問題</label><textarea id="fq"></textarea>
<label for="fa">答え</label><textarea id="fa"></textarea>
<label for="ft">この問題だけの制限時間（秒・空欄なら共通設定）</label>
<input type="number" id="ft" min="1" max="600">
<div class="row" style="margin-top:12px"><button class="btn" id="save">追加する</button><button class="btn alt" id="cancel" hidden>編集をやめる</button></div>
<p class="msg" id="formMsg"></p>
</div>
<div class="panel"><div id="list"></div></div>
<div class="row"><button class="btn alt sm" id="resetMarks">不正解の記録を消す</button><button class="btn alt sm" id="clearFlags">チェックをすべて外す</button></div>
</section>

<section id="io" hidden>
<div class="panel">
<b>ファイルから読み込む</b>
<p class="note">Excel（.xlsx）、CSV に対応。いま選んでいる問題集に追加されます（Excelに複数のシートがある場合は、シート名の問題集ごとに分けて読み込みます）。1行目に「問題」「答え」「制限秒」「チェック」の見出しを付けた表にしてください（制限秒・チェックは省略できます）。Google スプレッドシートは「ダウンロード」から .xlsx か .csv にして読み込めます。</p>
<input type="file" id="file" accept=".xlsx,.xls,.csv">
<p class="msg" id="ioMsg"></p>
</div>
<div class="panel">
<b>ファイルに書き出す</b>
<p class="note">書き出したファイルは、友だちに送ったりスプレッドシートに取り込んだりできます。</p>
<div class="row"><button class="btn" id="exX">この問題集をExcelで</button><button class="btn alt" id="exA">全問題集をExcelで（シートごと）</button><button class="btn alt" id="exC">CSV</button></div>
<div id="tsvBox" hidden><p class="note">この環境ではファイル保存が使えないため、下の表データをコピーしてスプレッドシートに貼り付けてください。</p><textarea id="tsv" readonly style="min-height:140px"></textarea></div>
<p class="msg" id="exMsg"></p>
</div>
</section>
</main>

<script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
<script>
const KEY = 'flashcards.v1';
let S = { cards: [], mode: 'all', limit: 20, shuffle: true };
try { const r = localStorage.getItem(KEY); if (r) S = Object.assign(S, JSON.parse(r)); } catch (e) {}
if (!Array.isArray(S.decks) || !S.decks.length) S.decks = [{ id: 'd1', name: '問題集1', cards: Array.isArray(S.cards) ? S.cards : [] }];
delete S.cards;
if (!S.decks.some(d => d.id === S.cur)) S.cur = S.decks[0].id;
const curDeck = () => S.decks.find(d => d.id === S.cur);
Object.defineProperty(S, 'cards', { get() { return curDeck().cards; }, set(v) { curDeck().cards = v; }, enumerable: false });
const $ = id => document.getElementById(id);
const persist = () => { try { localStorage.setItem(KEY, JSON.stringify(S)); } catch (e) {} };
const esc = s => String(s).replace(/&/g, '&amp;').replace(/</g, '&lt;').replace(/>/g, '&gt;');
const uid = () => Date.now().toString(36) + Math.random().toString(36).slice(2, 6);
let dl = null;
try { if (window.claude && claude.use) claude.use('downloads').then(d => { dl = d; }).catch(() => {}); } catch (e) {}

/* tabs */
document.querySelectorAll('nav button').forEach(b => b.onclick = () => {
  document.querySelectorAll('nav button').forEach(x => x.setAttribute('aria-selected', x === b));
  ['study', 'cards', 'io'].forEach(t => $(t).hidden = t !== b.dataset.tab);
  if (b.dataset.tab === 'cards') renderList();
  if (b.dataset.tab === 'study') refreshSetup();
});

/* decks */
function renderDecks(nm) {
  $('deck').innerHTML = S.decks.map(d => '<option value="' + d.id + '">' + esc(d.name) + '（' + d.cards.length + '問）</option>').join('');
  $('deck').value = S.cur;
  if (nm) $('dname').value = curDeck().name;
}
$('deck').onchange = () => { clearInterval(tm); R = null; S.cur = $('deck').value; persist(); clearForm(); renderDecks(true); refreshSetup(); renderList(); show('setup'); $('dMsg').textContent = ''; };
$('dNew').onclick = () => {
  let name = $('dname').value.trim();
  if (!name || name === curDeck().name) name = '問題集' + (S.decks.length + 1);
  const d = { id: uid(), name, cards: [] }; S.decks.push(d); S.cur = d.id;
  persist(); clearForm(); renderDecks(true); refreshSetup(); renderList();
  $('dMsg').textContent = '「' + name + '」を作りました。名前を変えるときは、入力欄を書き換えて「名前を変える」を押してください。';
};
$('dRen').onclick = () => {
  const name = $('dname').value.trim();
  if (!name) { $('dMsg').textContent = '名前を入力してください。'; return; }
  curDeck().name = name; persist(); renderDecks(true); $('dMsg').textContent = '名前を変えました。';
};
let armT = null;
$('dDel').onclick = () => {
  if (S.decks.length < 2) { $('dMsg').textContent = '最後の問題集は削除できません。'; return; }
  if (!armT) { $('dDel').textContent = 'もう一度押すと削除（' + S.cards.length + '問）'; armT = setTimeout(disarm, 4000); return; }
  const gone = curDeck().name; S.decks = S.decks.filter(d => d !== curDeck()); S.cur = S.decks[0].id;
  disarm(); persist(); clearForm(); renderDecks(true); refreshSetup(); renderList(); $('dMsg').textContent = '「' + gone + '」を削除しました。';
};
function disarm() { clearTimeout(armT); armT = null; $('dDel').textContent = 'この問題集を削除'; }
renderDecks(true);

/* setup */
function pool(mode) { return S.cards.filter(c => mode === 'flag' ? c.f : mode === 'wrong' ? c.w : true); }
function refreshSetup() {
  renderDecks();
  $('nAll').textContent = S.cards.length + '問';
  $('nFlag').textContent = pool('flag').length + '問';
  $('nWrong').textContent = pool('wrong').length + '問';
  document.querySelector('input[name=mode][value=' + S.mode + ']').checked = true;
  const presets = [0, 10, 20, 30, 60];
  if (presets.includes(S.limit)) { $('limit').value = S.limit; $('custom').hidden = true; }
  else { $('limit').value = 'x'; $('custom').hidden = false; $('custom').value = S.limit; }
  $('shuffle').checked = S.shuffle;
}
document.querySelectorAll('input[name=mode]').forEach(r => r.onchange = () => { S.mode = r.value; persist(); });
$('limit').onchange = () => {
  if ($('limit').value === 'x') { $('custom').hidden = false; $('custom').focus(); S.limit = +$('custom').value || 15; $('custom').value = S.limit; }
  else { $('custom').hidden = true; S.limit = +$('limit').value; }
  persist();
};
$('custom').oninput = () => { S.limit = Math.max(1, Math.min(600, +$('custom').value || 1)); persist(); };
$('shuffle').onchange = () => { S.shuffle = $('shuffle').checked; persist(); };

/* study */
let R = null, tm = null;
function show(id) { ['setup', 'play', 'result'].forEach(x => $(x).hidden = x !== id); }
function begin(mode) {
  const q = pool(mode).slice();
  if (!q.length) { $('setupMsg').textContent = mode === 'all' ? '問題がありません。「問題」タブで追加するか、ファイルを読み込んでください。' : mode === 'flag' ? 'チェックした問題がありません。' : '不正解の問題はありません。'; show('setup'); return; }
  $('setupMsg').textContent = '';
  if (S.shuffle) for (let i = q.length - 1; i > 0; i--) { const j = Math.floor(Math.random() * (i + 1)); [q[i], q[j]] = [q[j], q[i]]; }
  R = { q, i: 0, ok: 0, ng: 0, mode };
  show('play'); card();
}
function card() {
  const c = R.q[R.i];
  R.limit = c.t || S.limit; R.done = false;
  $('prog').textContent = (R.i + 1) + ' / ' + R.q.length;
  $('qText').textContent = c.q; $('aText').textContent = c.a;
  $('ans').hidden = true; $('tmsg').hidden = true;
  $('ctrl').hidden = false; $('judge').hidden = true; $('nextRow').hidden = true;
  flagUI(c);
  clearInterval(tm);
  const bar = $('bar');
  if (R.limit > 0) {
    R.t0 = performance.now(); tick();
    tm = setInterval(tick, 100);
  } else { bar.className = 'bar'; bar.firstElementChild.style.width = '100%'; $('left').textContent = '時間制限なし'; }
  $('reveal').focus();
}
function tick() {
  const left = R.limit - (performance.now() - R.t0) / 1000;
  const bar = $('bar');
  if (left <= 0) { clearInterval(tm); bar.firstElementChild.style.width = '0%'; $('left').textContent = '0秒'; return timeout(); }
  bar.firstElementChild.style.width = (left / R.limit * 100) + '%';
  bar.className = 'bar' + (left <= 3 ? ' crit' : left <= R.limit * 0.4 ? ' low' : '');
  $('left').textContent = 'あと ' + Math.ceil(left) + '秒';
}
function revealAns() { clearInterval(tm); $('ans').hidden = false; $('ctrl').hidden = true; }
$('reveal').onclick = () => { if (R.done) return; revealAns(); $('judge').hidden = false; $('okBtn').focus(); };
function timeout() {
  if (R.done) return; R.done = true;
  const c = R.q[R.i]; c.w = true; R.ng++; persist();
  revealAns(); $('tmsg').textContent = '時間切れ（不正解として記録しました）'; $('tmsg').hidden = false;
  $('nextRow').hidden = false; $('nextBtn').focus();
}
function judge(ok) {
  if (R.done) return; R.done = true;
  R.q[R.i].w = !ok; ok ? R.ok++ : R.ng++; persist(); next();
}
$('okBtn').onclick = () => judge(true);
$('ngBtn').onclick = () => judge(false);
$('nextBtn').onclick = next;
function next() { R.i++; R.i >= R.q.length ? finish() : card(); }
function finish() {
  clearInterval(tm); show('result');
  $('rOk').textContent = R.ok; $('rAll').textContent = R.q.length;
  $('rText').textContent = R.ng ? '不正解・時間切れは ' + R.ng + '問です。' : '全問正解です。';
  $('retryWrong').hidden = !pool('wrong').length;
}
$('quit').onclick = () => { clearInterval(tm); R = null; refreshSetup(); show('setup'); };
$('start').onclick = () => begin(S.mode);
$('again').onclick = () => begin(R.mode);
$('retryWrong').onclick = () => { S.mode = 'wrong'; persist(); begin('wrong'); };
$('back').onclick = () => { refreshSetup(); show('setup'); };
function flagUI(c) { const b = $('flagBtn'); b.setAttribute('aria-pressed', !!c.f); b.textContent = (c.f ? '★' : '☆') + ' チェック'; }
$('flagBtn').onclick = () => { const c = R.q[R.i]; c.f = !c.f; persist(); flagUI(c); };
document.addEventListener('keydown', e => {
  if (!R || $('play').hidden || /INPUT|TEXTAREA|SELECT/.test(e.target.tagName)) return;
  if (e.key === 'Enter' || e.key === ' ') { if (!$('ctrl').hidden) { e.preventDefault(); $('reveal').click(); } else if (!$('nextRow').hidden) { e.preventDefault(); $('nextBtn').click(); } }
  else if (e.key === '1' && !$('judge').hidden) judge(true);
  else if (e.key === '2' && !$('judge').hidden) judge(false);
});

/* cards */
let editId = null;
function renderList() {
  renderDecks();
  const el = $('list');
  if (!S.cards.length) { el.innerHTML = '<p class="note">まだ問題がありません。上のフォームから追加するか、「入出力」からファイルを読み込んでください。</p>'; return; }
  el.innerHTML = S.cards.map(c => '<div class="item"><b>' + esc(c.q) + '</b><small>' + esc(c.a) + '</small><div class="row" style="margin-top:6px">' +
    (c.f ? '<span class="tag" style="color:var(--flag)">チェック</span>' : '') + (c.w ? '<span class="tag" style="color:var(--ng)">不正解</span>' : '') + (c.t ? '<span class="tag" style="color:var(--sub)">' + c.t + '秒</span>' : '') +
    '<span class="grow"></span><button class="btn alt sm" data-a="flag" data-id="' + c.id + '">' + (c.f ? 'チェックを外す' : 'チェック') + '</button><button class="btn alt sm" data-a="edit" data-id="' + c.id + '">編集</button><button class="btn alt sm" data-a="del" data-id="' + c.id + '">削除</button></div></div>').join('');
}
$('list').onclick = e => {
  const b = e.target.closest('button'); if (!b) return;
  const c = S.cards.find(x => x.id === b.dataset.id); if (!c) return;
  if (b.dataset.a === 'flag') { c.f = !c.f; }
  else if (b.dataset.a === 'del') { S.cards = S.cards.filter(x => x !== c); if (editId === c.id) clearForm(); }
  else { editId = c.id; $('fq').value = c.q; $('fa').value = c.a; $('ft').value = c.t || ''; $('save').textContent = '更新する'; $('cancel').hidden = false; $('fq').focus(); window.scrollTo(0, 0); return; }
  persist(); renderList();
};
function clearForm() { editId = null; $('fq').value = ''; $('fa').value = ''; $('ft').value = ''; $('save').textContent = '追加する'; $('cancel').hidden = true; }
$('cancel').onclick = () => { clearForm(); $('formMsg').textContent = ''; };
$('save').onclick = () => {
  const q = $('fq').value.trim(), a = $('fa').value.trim(), t = Math.round(+$('ft').value) || 0;
  if (!q || !a) { $('formMsg').textContent = '問題と答えの両方を入力してください。'; return; }
  const c = editId && S.cards.find(x => x.id === editId);
  if (c) { c.q = q; c.a = a; c.t = t; $('formMsg').textContent = '更新しました。'; }
  else { S.cards.push({ id: uid(), q, a, t, f: false, w: false }); $('formMsg').textContent = '追加しました（全' + S.cards.length + '問）。'; }
  clearForm(); persist(); renderList(); $('fq').focus();
};
$('resetMarks').onclick = () => { S.cards.forEach(c => c.w = false); persist(); renderList(); };
$('clearFlags').onclick = () => { S.cards.forEach(c => c.f = false); persist(); renderList(); };

/* import */
const truthy = v => ['○', '〇', '◯', '✓', '1', 'true', 'yes', 'y', 'チェック'].includes(String(v == null ? '' : v).trim().toLowerCase());
$('file').onchange = async e => {
  const f = e.target.files[0]; if (!f) return;
  const m = $('ioMsg'); m.textContent = '読み込み中…';
  try {
    if (typeof XLSX === 'undefined') throw new Error('lib');
    const buf = await f.arrayBuffer();
    let wb;
    if (/\.csv$/i.test(f.name)) {
      let txt = new TextDecoder('utf-8').decode(buf);
      if (txt.includes('\uFFFD')) txt = new TextDecoder('shift_jis').decode(buf);
      wb = XLSX.read(txt, { type: 'string' });
    } else wb = XLSX.read(buf, { type: 'array' });
    let n = 0, skip = 0, made = 0;
    const multi = wb.SheetNames.length > 1;
    for (const sn of wb.SheetNames) {
    const rows = XLSX.utils.sheet_to_json(wb.Sheets[sn], { header: 1, blankrows: false, defval: '' });
    let target = S.cards;
    if (multi) { let d = S.decks.find(x => x.name === sn); if (!d) { d = { id: uid(), name: sn, cards: [] }; S.decks.push(d); made++; } target = d.cards; }
    let start = 0;
    if (rows.length && ['問題', 'question', 'q'].includes(String(rows[0][0]).trim().toLowerCase())) start = 1;
    for (const r of rows.slice(start)) {
      const q = String(r[0] == null ? '' : r[0]).trim(), a = String(r[1] == null ? '' : r[1]).trim();
      if (!q || !a) { skip++; continue; }
      target.push({ id: uid(), q, a, t: Math.round(+r[2]) || 0, f: truthy(r[3]), w: false }); n++;
    }
    }
    persist(); renderList(); refreshSetup();
    m.textContent = (made ? made + '個の問題集を作り、' : '') + n + '問を追加しました' + (skip ? '（問題か答えが空の ' + skip + '行は飛ばしました）' : '') + '。';
  } catch (err) { m.textContent = '読み込めませんでした。.xlsx か .csv で、1列目が問題、2列目が答えの表か確認してください。'; }
  e.target.value = '';
};

/* export */
function tableOf(cs) { return [['問題', '答え', '制限秒', 'チェック']].concat(cs.map(c => [c.q, c.a, c.t || '', c.f ? '○' : ''])); }
function table() { return tableOf(S.cards); }
async function out(kind) {
  const m = $('exMsg'); m.textContent = '';
  if (!(kind === 'a' ? S.decks.some(d => d.cards.length) : S.cards.length)) { m.textContent = '書き出す問題がありません。'; return; }
  const aoa = table();
  if (!dl || typeof XLSX === 'undefined') {
    $('tsv').value = aoa.map(r => r.map(v => String(v).replace(/[\t\r\n]+/g, ' ')).join('\t')).join('\n');
    $('tsvBox').hidden = false; return;
  }
  try {
    const ws = XLSX.utils.aoa_to_sheet(aoa);
    if (kind === 'x' || kind === 'a') {
      const wb = XLSX.utils.book_new();
      if (kind === 'a') { const used = {}; S.decks.forEach((d, i) => { let nm = d.name.replace(/[\[\]:*?\/\\]/g, ' ').slice(0, 28) || '問題集' + (i + 1); while (used[nm]) nm = nm.slice(0, 25) + '_' + i; used[nm] = 1; XLSX.utils.book_append_sheet(wb, XLSX.utils.aoa_to_sheet(tableOf(d.cards)), nm); }); }
      else XLSX.utils.book_append_sheet(wb, ws, '問題');
      await dl.save({ filename: (kind === 'a' ? '暗記カード全問題集' : curDeck().name) + '.xlsx', data: XLSX.write(wb, { bookType: 'xlsx', type: 'array' }) });
    } else await dl.save({ filename: curDeck().name + '.csv', data: '\uFEFF' + XLSX.utils.sheet_to_csv(ws) });
    m.textContent = '保存しました。';
  } catch (err) { m.textContent = err && err.code === 'declined' ? '保存をキャンセルしました。' : '保存できませんでした。もう一度お試しください。'; }
}
$('exX').onclick = () => out('x');
$('exC').onclick = () => out('c');
$('exA').onclick = () => out('a');

refreshSetup(); show('setup');
</script>
</body>
</html>
