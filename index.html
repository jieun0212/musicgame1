<!doctype html>
<html lang="ko">
<head>
<meta charset="utf-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>신호등 음악게임</title>
<style>
:root{--bg:#f6f7fb;--card:#fff;--ink:#172033;--muted:#687386;--blue:#3559d8}
*{box-sizing:border-box}body{margin:0;background:var(--bg);font-family:system-ui,-apple-system,"Noto Sans KR",sans-serif;color:var(--ink)}
.app{max-width:1180px;margin:auto;padding:22px}.head{text-align:center}.head h1{font-size:38px;margin:4px}.rule{font-size:20px;color:var(--muted);font-weight:700}
.tabs{display:flex;justify-content:center;gap:10px;margin:20px}.tab{border:0;padding:12px 22px;border-radius:14px;font-size:17px;font-weight:850;cursor:pointer}.tab.on{background:var(--blue);color:white}
.board{background:white;border-radius:24px;padding:24px;box-shadow:0 10px 35px #00000010}
.main{display:grid;grid-template-columns:minmax(0,3fr) minmax(175px,1fr);gap:30px;align-items:center;min-height:430px}
.staffbox{position:relative}.staff{width:100%;height:auto;aspect-ratio:280 / 290;display:block}.noteName{text-align:center;font-size:34px;font-weight:900;min-height:48px}
.light{width:175px;background:#222a36;border-radius:38px;padding:25px 22px;margin:auto;box-shadow:inset 0 0 0 5px #1117}
.bulb{width:125px;height:125px;border-radius:50%;margin:10px auto;transition:.2s}.red{background:#421d22}.green{background:#153c2a}.red.on{background:#ff334d;box-shadow:0 0 32px #ff334daa}.green.on{background:#20d875;box-shadow:0 0 32px #20d875aa}
.counter{text-align:center;font-size:20px;font-weight:850;margin-top:16px}
.controls,.settings{display:flex;flex-wrap:wrap;justify-content:center;gap:9px;margin-top:18px}.btn{border:0;border-radius:13px;padding:12px 16px;font-size:16px;font-weight:850;cursor:pointer;background:#e8ebf2}.primary{background:var(--blue);color:white}.nameBtn{background:#fff3cd}
.settings{border-top:1px solid #e6e8ee;padding-top:17px}.group{display:flex;align-items:center;gap:5px;background:#f1f3f7;padding:5px;border-radius:13px}.group strong{padding:0 7px}.choice{border:0;background:transparent;padding:8px 10px;border-radius:9px;font-weight:800;cursor:pointer}.choice.on{background:white;box-shadow:0 2px 8px #0001;color:var(--blue)}
@media(max-width:760px){.main{grid-template-columns:1fr;gap:5px}.staff{height:auto}.light{display:flex;width:270px;padding:12px 18px}.bulb{width:95px;height:95px}.head h1{font-size:30px}.board{padding:10px}}

.notePicker{display:flex;flex-wrap:wrap;justify-content:center;gap:6px;margin-top:12px}
.notePick{border:2px solid #d9dde7;background:white;border-radius:10px;padding:7px 10px;font-weight:800;cursor:pointer}
.notePick.on{border-color:#3559d8;background:#eef2ff}
.hidden{display:none!important}
.answerFlash{font-size:42px;font-weight:950;text-align:center;min-height:56px;margin-top:4px}
.smallhint{text-align:center;color:#687386;font-size:14px;margin-top:8px}

.introScreen{min-height:100vh;display:flex;align-items:center;justify-content:center;padding:24px;background:linear-gradient(150deg,#edf2ff,#f7f9fd 55%,#e8fff2)}
.introCard{width:min(850px,100%);background:white;border-radius:28px;padding:48px 40px;text-align:center;box-shadow:0 20px 65px #25345a18}
.introTag{display:inline-block;border-radius:100px;padding:8px 15px;background:#edf2ff;color:#3559d8;font-weight:850}
.introCard h1{font-size:clamp(32px,5vw,52px);letter-spacing:-1.5px;margin:20px 0 10px}
.introLead{font-size:19px;color:#687386;line-height:1.7}
.introRules{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin:30px 0}
.introRule{background:#f6f7fb;border-radius:18px;padding:23px 14px;text-align:left}
.introRule .symbol{font-size:32px}.introRule h3{margin:10px 0 8px;font-size:18px}.introRule p{margin:0;color:#687386;line-height:1.6;font-size:15px}
.introStart{border:0;border-radius:15px;background:#3559d8;color:white;padding:17px 40px;font-size:20px;font-weight:900;cursor:pointer}
.introHidden{display:none!important}
@media(max-width:650px){.introCard{padding:32px 20px}.introRules{grid-template-columns:1fr}.introRule{text-align:center}}

/* 전자칠판 한 화면용 레이아웃 */
.app{max-width:1250px;padding:14px 18px 22px}
.head h1{font-size:30px;margin:0 0 2px}
.rule{font-size:17px}
.tabs{margin:7px 0;gap:8px}
.tab{padding:8px 17px;font-size:16px}
.board{padding:22px 22px 24px;border-radius:22px}
.main{grid-template-columns:minmax(0,1fr) 185px;gap:18px;min-height:470px;align-items:center}
.staffbox{display:flex;flex-direction:column;align-items:center;justify-content:center;min-width:0}
.staff{width:min(100%,800px);height:auto;aspect-ratio:520 / 285;flex:none}
.noteName{font-size:clamp(42px,4.5vw,64px);min-height:0;line-height:1.15;margin:0 0 8px;font-weight:950}
.noteName:empty,.answerFlash:empty{display:none}
.answerFlash{font-size:clamp(42px,4.5vw,64px);min-height:0;line-height:1.15;margin:0}
.light{width:146px;padding:14px 12px;border-radius:30px}
.bulb{width:108px;height:108px;margin:7px auto}
.counter{font-size:18px;margin-top:9px}
.controls,.settings{margin-top:14px;gap:8px}
.controls{padding-top:14px}
.btn{padding:9px 12px;font-size:15px}
.settings{padding-top:10px}
.group{padding:3px}
.choice{padding:7px 8px}
.notePicker{margin-top:11px;gap:6px}
.notePick{padding:5px 8px}
.smallhint{margin-top:5px;font-size:12px}
@media(max-width:760px){
 .main{grid-template-columns:1fr;gap:3px}
 .staff{width:min(100%,520px);height:auto}
 .light{display:flex;width:190px;padding:8px;gap:8px;border-radius:20px}
 .bulb{width:74px;height:74px;margin:3px auto}
 .head h1{font-size:25px}
 .board{padding:10px}
}
@media(min-width:900px) and (max-height:760px){
 .staff{height:auto;width:min(100%,690px)}
 .bulb{width:90px;height:90px}
 .light{width:128px;padding:9px}
 .head h1{font-size:27px}
 .tab{padding:6px 14px}
}
</style></head>
<body>
<section id="introScreen" class="introScreen">
 <div class="introCard">
  <span class="introTag">🎵 음악수업 · 오선지 읽기</span>
  <h1>🚦 신호등 음악게임</h1>
  <p class="introLead">음표를 보고, 신호등을 확인하고, 알맞게 연주해 보세요!<br>눈으로 음을 읽고 빠르게 판단하는 음악 활동이에요.</p>
  <div class="introRules">
   <div class="introRule"><div class="symbol">🎼</div><h3>① 음표를 살펴봐요</h3><p>오선지에 나타난 음표가 어떤 음인지 확인해요.</p></div>
   <div class="introRule"><div class="symbol">🟢</div><h3>② 초록불이면 연주!</h3><p>초록불이 켜지면 보이는 음을 악기로 연주해요.</p></div>
   <div class="introRule"><div class="symbol">🔴</div><h3>③ 빨간불이면 멈춰요!</h3><p>빨간불이 켜지면 악기를 연주하지 않고 기다려요.</p></div>
  </div>
  <p class="introLead" style="font-size:16px"><strong>💡 이렇게도 활용해요!</strong><br>악기 없이도 게임에 참여할 수 있어요! 초록불이 켜지면 악보를 보고 음이름을 소리 내어 읽고, 빨간불이 켜지면 읽지 않고 기다려요.</p>
  <p class="introLead" style="font-size:16px">익숙해지면 <strong>화음 모드</strong>에도 도전할 수 있어요.</p>
  <button class="introStart" id="enterGame">게임하러 가기 →</button>
 </div>
</section>
<div class="app introHidden" id="gameApp">
<header class="head"><h1>🚦 신호등 음악게임</h1><div class="rule">🟢 연주해요!　 🔴 연주하지 않아요!</div></header>
<div class="tabs"><button class="tab on" id="singleTab">🎵 한 음</button><button class="tab" id="chordTab">🎶 번외 · 화음</button></div>
<section class="board">
<div class="main">
 <div class="staffbox"><svg class="staff" id="staff" viewBox="0 20 520 285" aria-label="오선지"></svg><div class="noteName" id="noteName"></div></div>
 <div><div class="light"><div class="bulb red" id="red"></div><div class="bulb green" id="green"></div></div><div class="counter" id="counter">게임을 시작해 주세요</div></div>
</div>
<div class="controls">
 <button class="btn primary" id="start">▶ 게임 시작</button>
 <button class="btn primary" id="next">⏭ 다음 문제</button>
 <button class="btn" id="reset">🔄 처음부터</button>
 <button class="btn nameBtn" id="showName">👀 음이름 보기</button>
 <button class="btn" id="backIntro">↩ 게임 설명으로</button>
 
</div>
<div class="settings">
 <div class="group"><strong>음 범위</strong><button class="choice" data-range="2">도~미</button><button class="choice on" data-range="4">도~솔</button><button class="choice" data-range="7">도~높은 도</button><button class="choice" data-range="9">도~높은 미</button><button class="choice" data-range="14">도~2옥타브 도</button></div>
 <div class="group"><strong>신호등</strong><button class="choice lightChoice on" data-green=".7">🟢 많이</button><button class="choice lightChoice" data-green=".5">1:1</button><button class="choice lightChoice" data-green=".3">🔴 많이</button></div>
 <div class="group chordSettings hidden" id="chordSettings"><strong>화음</strong><button class="choice chordChoice" data-chord="third">3도</button><button class="choice chordChoice" data-chord="fifth">5도</button><button class="choice chordChoice on" data-chord="mix">3·5도 섞기</button></div>
</div>
<div class="notePicker" id="notePicker"></div>
<div class="smallhint">개별 음을 눌러 출제 여부를 선택할 수 있어요. 음 범위를 누르면 해당 범위가 자동 선택됩니다.</div></div>
</section></div>
<script>
document.getElementById("enterGame").addEventListener("click",()=>{
 document.getElementById("introScreen").classList.add("introHidden");
 document.getElementById("gameApp").classList.remove("introHidden");
 window.scrollTo(0,0);
});
document.getElementById("backIntro").addEventListener("click",()=>{
 document.getElementById("gameApp").classList.add("introHidden");
 document.getElementById("introScreen").classList.remove("introHidden");
 window.scrollTo(0,0);
});
const NS="http://www.w3.org/2000/svg";
const notes=[
 {n:"도",y:272,c:"#ef4444"},{n:"레",y:256,c:"#f97316"},{n:"미",y:240,c:"#facc15"},{n:"파",y:224,c:"#84cc16"},{n:"솔",y:208,c:"#38bdf8"},
 {n:"라",y:192,c:"#1e3a8a"},{n:"시",y:176,c:"#8b5cf6"},{n:"높은 도",y:160,c:"#ef4444"},{n:"높은 레",y:144,c:"#f97316"},{n:"높은 미",y:128,c:"#facc15"},
 {n:"높은 파",y:112,c:"#84cc16"},{n:"높은 솔",y:96,c:"#38bdf8"},{n:"높은 라",y:80,c:"#1e3a8a"},{n:"높은 시",y:64,c:"#8b5cf6"},{n:"2옥타브 도",y:48,c:"#ef4444"}
];
let maxIdx=4,total=0,num=0,mode="single",current=[],light="green",showing=false,started=false,paused=false;
let greenProb=.7,chordType="mix";
let selected=new Set([0,1,2,3,4]);

function E(tag,attrs={}){let e=document.createElementNS(NS,tag);for(const[k,v]of Object.entries(attrs))e.setAttribute(k,v);return e}

function renderPicker(){
 notePicker.innerHTML="";
 notes.forEach((nt,i)=>{
   const b=document.createElement("button");
   b.className="notePick"+(selected.has(i)?" on":"");
   b.textContent=nt.n;
   b.style.color=nt.c;
   b.onclick=()=>{
     if(selected.has(i)){
       if(selected.size<=1)return;
       selected.delete(i);
     }else selected.add(i);
     renderPicker();
   };
   notePicker.appendChild(b);
 });
}
function clearSignal(){
 red.classList.remove("on");green.classList.remove("on");
}
function draw(){
 staff.innerHTML="";
 // five staff lines: E4(240) to F5(112); 32px spacing
 [240,208,176,144,112].forEach(y=>staff.appendChild(E("line",{x1:40,y1:y,x2:480,y2:y,stroke:"#172033","stroke-width":3})));
 // left bar
 staff.appendChild(E("line",{x1:40,y1:112,x2:40,y2:240,stroke:"#172033","stroke-width":4}));

 current.forEach((idx,j)=>{
   let {y}=notes[idx],x=260;
   // 오선 밖의 음에 필요한 덧줄 표시
   if(y===272) staff.appendChild(E("line",{x1:x-36,y1:272,x2:x+36,y2:272,stroke:"#172033","stroke-width":3}));
   [80,48].forEach(ly=>{if(y<=ly) staff.appendChild(E("line",{x1:x-36,y1:ly,x2:x+36,y2:ly,stroke:"#172033","stroke-width":3}));});
   // 음표 기둥 없이 검은 음표 머리(동그라미)만 표시
   let head=E("ellipse",{cx:x,cy:y,rx:18,ry:14,fill:notes[idx].c,stroke:"#172033","stroke-width":1.5}); staff.appendChild(head);
 });
 noteName.textContent=showing&&current.length?current.map(i=>notes[i].n).join(" + "):"";
}
function choose(){
 if(!started||paused)return;
 
 const pool=[...selected].sort((a,b)=>a-b);
 if(!pool.length)return;
 num++;clearSignal();current=[];
 if(mode==="single"){
   current=[pool[Math.floor(Math.random()*pool.length)]];
 }else{
   const intervals=chordType==="third"?[2]:chordType==="fifth"?[4]:[2,4];
   const pairs=[];
   pool.forEach(root=>intervals.forEach(iv=>{
     const upper=root+iv;
     if(selected.has(upper))pairs.push([root,upper]);
   }));
   if(!pairs.length){
     counter.textContent="선택한 음 안에 가능한 화음이 없어요";
     num--;return;
   }
   current=pairs[Math.floor(Math.random()*pairs.length)];
 }
 light=Math.random()<greenProb?"green":"red";
 red.classList.toggle("on",light==="red");green.classList.toggle("on",light==="green");
 showName.textContent=showing?"🙈 음이름 숨기기":"👀 음이름 보기";
 counter.textContent=`${num}번째 문제`;draw();
}
function begin(){
 started=true;paused=false;num=0;counter.textContent="3";current=[];clearSignal();draw();
 setTimeout(()=>{if(started&&!paused){counter.textContent="2";setTimeout(()=>{if(started&&!paused){counter.textContent="1";setTimeout(choose,600)}},600)}},600);
}
start.onclick=begin;next.onclick=choose;
reset.onclick=()=>{started=false;paused=false;num=0;current=[];showing=false;red.classList.remove("on");green.classList.remove("on");counter.textContent="게임을 시작해 주세요";draw()};
showName.onclick=()=>{if(!current.length)return;showing=!showing;showName.textContent=showing?"🙈 음이름 숨기기":"👀 음이름 보기";draw()};

singleTab.onclick=()=>{mode="single";singleTab.classList.add("on");chordTab.classList.remove("on");chordSettings.classList.add("hidden");if(started)choose();else draw()};
chordTab.onclick=()=>{mode="chord";chordTab.classList.add("on");singleTab.classList.remove("on");chordSettings.classList.remove("hidden");if(started)choose();else draw()};
document.querySelectorAll("[data-range]").forEach(b=>b.onclick=()=>{
 maxIdx=+b.dataset.range;selected=new Set(Array.from({length:maxIdx+1},(_,i)=>i));renderPicker();
 document.querySelectorAll("[data-range]").forEach(x=>x.classList.toggle("on",x===b))
});
document.querySelectorAll(".lightChoice").forEach(b=>b.onclick=()=>{greenProb=+b.dataset.green;document.querySelectorAll(".lightChoice").forEach(x=>x.classList.toggle("on",x===b))});
document.querySelectorAll(".chordChoice").forEach(b=>b.onclick=()=>{chordType=b.dataset.chord;document.querySelectorAll(".chordChoice").forEach(x=>x.classList.toggle("on",x===b))});
renderPicker();draw();
</script></body></html>
