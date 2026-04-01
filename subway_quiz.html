<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>지하철 퀴즈</title>
<style>
  *{box-sizing:border-box;margin:0;padding:0}
  body{font-family:-apple-system,'Apple SD Gothic Neo',sans-serif;background:#f2f2f7;display:flex;justify-content:center;min-height:100vh}
  .phone{width:100%;max-width:390px;min-height:100vh;background:#fff;display:flex;flex-direction:column;position:relative}

  .hdr{padding:16px 20px 12px;background:#fff;border-bottom:1px solid #f0f0f0;display:flex;align-items:center;justify-content:space-between}
  .hdr-title{font-size:17px;font-weight:600;color:#111}
  .hdr-stage{font-size:12px;color:#888}
  .lives{display:flex;gap:3px}
  .heart{font-size:16px}
  .score-display{font-size:22px;font-weight:700;color:#111}

  .ad-banner{height:50px;background:#f8f8f8;border-top:1px solid #e8e8e8;display:flex;align-items:center;justify-content:center;flex-shrink:0}
  .ad-banner span{font-size:11px;color:#bbb;letter-spacing:.05em}

  .screen{flex:1;display:none;flex-direction:column;overflow-y:auto}
  .screen.active{display:flex}

  /* HOME */
  .home-hero{padding:32px 24px 20px;text-align:center}
  .home-hero .icon{font-size:52px;margin-bottom:12px}
  .home-hero h1{font-size:24px;font-weight:700;color:#111;margin-bottom:6px}
  .home-hero p{font-size:14px;color:#888;line-height:1.6}

  /* daily card */
  .daily-card{margin:0 20px 16px;border-radius:18px;padding:18px 20px;background:linear-gradient(135deg,#1a1a2e,#16213e);cursor:pointer;position:relative;overflow:hidden;transition:transform .1s}
  .daily-card:active{transform:scale(.98)}
  .daily-card.done{opacity:.6;cursor:default}
  .daily-card:active.done{transform:none}
  .dc-label{font-size:11px;font-weight:600;color:#7F77DD;letter-spacing:.08em;margin-bottom:6px}
  .dc-title{font-size:18px;font-weight:700;color:#fff;margin-bottom:4px}
  .dc-sub{font-size:12px;color:#aaa}
  .dc-badge{position:absolute;top:16px;right:16px;background:#4CAF50;color:#fff;font-size:11px;font-weight:600;padding:4px 10px;border-radius:99px}
  .dc-hint-row{display:flex;align-items:center;gap:6px;margin-top:12px}
  .dc-hint-chip{background:rgba(255,255,255,.12);color:#ddd;font-size:11px;padding:4px 10px;border-radius:99px}

  .stage-list{padding:0 20px 24px;display:flex;flex-direction:column;gap:10px}
  .section-label{font-size:11px;font-weight:600;color:#aaa;letter-spacing:.06em;margin:4px 0 8px}
  .stage-card{border-radius:16px;padding:16px 18px;display:flex;align-items:center;gap:14px;cursor:pointer;transition:transform .1s;border:1.5px solid transparent}
  .stage-card:active{transform:scale(.98)}
  .stage-card.locked{opacity:.4;cursor:default}
  .stage-card.locked:active{transform:none}
  .sc-icon{width:42px;height:42px;border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:20px;flex-shrink:0}
  .sc-info{flex:1}
  .sc-info .sc-name{font-size:15px;font-weight:600;margin-bottom:2px}
  .sc-info .sc-desc{font-size:12px}
  .sc-stars{font-size:15px;letter-spacing:1px}
  .s1{background:#E8F5E9;border-color:#A5D6A7}.s1 .sc-icon{background:#4CAF50}.s1 .sc-name{color:#2E7D32}.s1 .sc-desc{color:#558B2F}
  .s2{background:#E3F2FD;border-color:#90CAF9}.s2 .sc-icon{background:#2196F3}.s2 .sc-name{color:#1565C0}.s2 .sc-desc{color:#1976D2}
  .s3{background:#FFF3E0;border-color:#FFCC80}.s3 .sc-icon{background:#FF9800}.s3 .sc-name{color:#E65100}.s3 .sc-desc{color:#F57C00}
  .sb{background:#FCE4EC;border-color:#F48FB1}.sb .sc-icon{background:#E91E63}.sb .sc-name{color:#880E4F}.sb .sc-desc{color:#C2185B}

  /* QUIZ */
  .quiz-progress{padding:14px 20px 8px}
  .prog-bar{height:6px;background:#f0f0f0;border-radius:3px;overflow:hidden}
  .prog-fill{height:100%;border-radius:3px;transition:width .4s}
  .prog-info{display:flex;justify-content:space-between;margin-top:6px;font-size:12px;color:#999}

  .quiz-body{padding:16px 20px;flex:1;display:flex;flex-direction:column}
  .quiz-type-badge{display:inline-flex;align-items:center;gap:5px;font-size:11px;font-weight:600;padding:4px 10px;border-radius:99px;margin-bottom:14px}
  .badge-a{background:#E3F2FD;color:#1565C0}
  .badge-b{background:#FFF8E1;color:#F57F17}

  .line-indicator{display:flex;align-items:center;gap:8px;margin-bottom:16px}
  .line-dot{width:28px;height:28px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:13px;font-weight:700;color:#fff;flex-shrink:0}
  .line-name{font-size:13px;font-weight:600;color:#555}

  .question-card{background:#f8f8f8;border-radius:16px;padding:20px;margin-bottom:20px}
  .question-card .q-label{font-size:12px;color:#999;margin-bottom:6px}
  .question-card .q-station{font-size:22px;font-weight:700;color:#111;margin-bottom:4px}
  .question-card .q-sub{font-size:13px;color:#777}

  .chosung-box{background:#fff;border:2px solid #e0e0e0;border-radius:12px;padding:14px 20px;text-align:center;margin-bottom:8px}
  .chosung-text{font-size:28px;font-weight:700;letter-spacing:8px;color:#333}
  .chosung-hint{font-size:12px;color:#aaa;margin-top:4px}

  .options{display:flex;flex-direction:column;gap:10px;margin-top:4px}
  .opt-btn{padding:15px 18px;border-radius:14px;border:1.5px solid #e8e8e8;background:#fff;font-size:15px;font-weight:500;color:#222;text-align:left;cursor:pointer;transition:all .15s;display:flex;align-items:center;gap:10px}
  .opt-btn:active{transform:scale(.98)}
  .opt-btn.eliminated{opacity:.3;pointer-events:none;text-decoration:line-through}
  .opt-num{width:24px;height:24px;border-radius:50%;background:#f0f0f0;display:flex;align-items:center;justify-content:center;font-size:12px;font-weight:600;color:#888;flex-shrink:0}
  .opt-btn.correct{background:#E8F5E9;border-color:#4CAF50}
  .opt-btn.correct .opt-num{background:#4CAF50;color:#fff}
  .opt-btn.wrong{background:#FFEBEE;border-color:#EF5350}
  .opt-btn.wrong .opt-num{background:#EF5350;color:#fff}

  .chosung-input-wrap{display:flex;flex-direction:column;gap:10px}
  .chosung-input{width:100%;padding:14px 16px;border-radius:14px;border:1.5px solid #e0e0e0;font-size:18px;font-weight:600;text-align:center;color:#111;outline:none;transition:border-color .2s}
  .chosung-input:focus{border-color:#2196F3}
  .chosung-input.correct{border-color:#4CAF50;background:#E8F5E9;color:#2E7D32}
  .chosung-input.wrong{border-color:#EF5350;background:#FFEBEE;color:#C62828}
  .submit-btn{padding:14px;border-radius:14px;background:#2196F3;color:#fff;font-size:15px;font-weight:600;border:none;cursor:pointer}
  .submit-btn:disabled{background:#ccc;cursor:default}

  /* hint bar */
  .hint-bar{display:flex;align-items:center;justify-content:flex-end;margin-bottom:12px;gap:8px}
  .hint-count{font-size:12px;color:#888}
  .hint-btn{display:flex;align-items:center;gap:5px;padding:7px 13px;border-radius:99px;border:1.5px solid #FF9800;background:#FFF8E1;color:#E65100;font-size:12px;font-weight:600;cursor:pointer;transition:all .15s}
  .hint-btn:active{background:#FFE0B2}
  .hint-btn.disabled{opacity:.4;cursor:default;pointer-events:none}
  .hint-ad-btn{padding:7px 13px;border-radius:99px;border:1.5px solid #9E9E9E;background:#f5f5f5;color:#555;font-size:12px;font-weight:600;cursor:pointer}

  .feedback{text-align:center;padding:10px 0;font-size:14px;font-weight:600;min-height:24px}
  .feedback.correct{color:#4CAF50}
  .feedback.wrong{color:#EF5350}

  /* RESULT */
  .result-wrap{flex:1;display:flex;flex-direction:column;align-items:center;justify-content:center;padding:32px 24px;text-align:center}
  .result-emoji{font-size:64px;margin-bottom:16px}
  .result-title{font-size:24px;font-weight:700;color:#111;margin-bottom:8px}
  .result-sub{font-size:14px;color:#888;margin-bottom:24px;line-height:1.7;white-space:pre-line}
  .result-score{font-size:42px;font-weight:800;color:#111;margin-bottom:4px}
  .result-score-label{font-size:13px;color:#aaa;margin-bottom:20px}
  .stars-display{font-size:36px;letter-spacing:4px;margin-bottom:28px}
  .result-btns{display:flex;flex-direction:column;gap:10px;width:100%}
  .btn-primary{padding:15px;border-radius:14px;background:#111;color:#fff;font-size:15px;font-weight:600;border:none;cursor:pointer}
  .btn-secondary{padding:15px;border-radius:14px;background:#f0f0f0;color:#333;font-size:15px;font-weight:600;border:none;cursor:pointer}

  /* daily result extra */
  .daily-result-badge{background:#1a1a2e;color:#7F77DD;font-size:13px;font-weight:600;padding:8px 18px;border-radius:99px;margin-bottom:20px;display:inline-block}

  .combo-badge{position:fixed;top:80px;left:50%;transform:translateX(-50%);background:#FF6F00;color:#fff;padding:6px 16px;border-radius:99px;font-size:13px;font-weight:700;opacity:0;transition:opacity .3s;pointer-events:none;z-index:99}
  .combo-badge.show{opacity:1}

  /* toast */
  .toast{position:fixed;bottom:80px;left:50%;transform:translateX(-50%);background:rgba(0,0,0,.8);color:#fff;padding:10px 18px;border-radius:99px;font-size:13px;opacity:0;transition:opacity .3s;pointer-events:none;z-index:100;white-space:nowrap}
  .toast.show{opacity:1}
</style>
</head>
<body>
<div class="phone">
  <div class="combo-badge" id="comboBadge">🔥 콤보!</div>
  <div class="toast" id="toast"></div>

  <!-- HOME -->
  <div class="screen active" id="screenHome">
    <div class="hdr">
      <span class="hdr-title">🚇 지하철 퀴즈</span>
      <span class="score-display" id="totalScore">0점</span>
    </div>
    <div class="home-hero">
      <div class="icon">🗺️</div>
      <h1>노선도 퀴즈</h1>
      <p>서울 지하철 역을 얼마나 알고 있나요?</p>
    </div>
    <div id="dailyCardWrap" style="margin-bottom:4px"></div>
    <div class="stage-list">
      <div class="section-label">STAGES</div>
      <div id="stageList"></div>
    </div>
    <div class="ad-banner"><span>AD BANNER</span></div>
  </div>

  <!-- QUIZ -->
  <div class="screen" id="screenQuiz">
    <div class="hdr">
      <div>
        <div class="hdr-title" id="quizStageName"></div>
        <div class="hdr-stage" id="quizStageDesc"></div>
      </div>
      <div style="display:flex;align-items:center;gap:12px">
        <div class="lives" id="livesDisplay"></div>
        <div class="score-display" id="quizScore">0</div>
      </div>
    </div>
    <div class="quiz-progress">
      <div class="prog-bar"><div class="prog-fill" id="progFill" style="width:0%"></div></div>
      <div class="prog-info"><span id="progText">1/5</span><span id="progCorrect">정답 0</span></div>
    </div>
    <div class="quiz-body" id="quizBody"></div>
    <div class="ad-banner"><span>AD BANNER</span></div>
  </div>

  <!-- RESULT -->
  <div class="screen" id="screenResult">
    <div class="result-wrap" id="resultWrap"></div>
    <div class="ad-banner"><span>AD BANNER</span></div>
  </div>
</div>

<script>
// ── DATA ──
const LINES = {
  '1':{name:'1호선',color:'#0052A4'},'2':{name:'2호선',color:'#00A84D'},
  '3':{name:'3호선',color:'#EF7C1C'},'4':{name:'4호선',color:'#00A5DE'},
  '5':{name:'5호선',color:'#996CAC'},'6':{name:'6호선',color:'#CD7C2F'},
  '7':{name:'7호선',color:'#747F00'},'8':{name:'8호선',color:'#E6186C'},
  '9':{name:'9호선',color:'#BDB092'},
};
// [line, station, prev, next]
const STATIONS=[
  ['1','서울역','남영','시청'],['1','종각','시청','종로3가'],['1','동대문','종로5가','신설동'],
  ['1','청량리','제기동','회기'],['1','수원','성균관대','화서'],['1','인천','도원','동인천'],
  ['2','강남','역삼','삼성'],['2','홍대입구','합정','신촌'],['2','신촌','홍대입구','이대'],
  ['2','을지로3가','을지로입구','을지로4가'],['2','잠실','송파','잠실나루'],
  ['2','서울대입구','낙성대','사당'],['2','건대입구','구의','성수'],
  ['3','경복궁','안국','종로3가'],['3','교대','남부터미널','양재'],
  ['3','고속터미널','반포','잠원'],['3','양재','교대','매봉'],['3','도곡','매봉','대치'],
  ['4','명동','회현','충무로'],['4','동대문역사문화공원','동대문','신당'],
  ['4','사당','총신대입구','남태령'],['4','혜화','한성대입구','성신여대입구'],
  ['5','광화문','종로3가','서대문'],['5','여의도','마포','공덕'],
  ['5','왕십리','마장','행당'],['5','강동','길동','천호'],
  ['6','이태원','한강진','녹사평'],['6','합정','망원','상수'],
  ['6','디지털미디어시티','월드컵경기장','증산'],
  ['7','강남구청','학동','뚝섬유원지'],['7','노원','중계','하계'],['7','이수','남성','숭실대입구'],
  ['8','잠실','석촌','몽촌토성'],['8','천호','강동구청','암사'],
  ['9','김포공항','공항시장','신방화'],['9','봉은사','삼성중앙','종합운동장'],['9','여의도','샛강','국회의사당'],
];
const STAGES=[
  {id:1,name:'입문',desc:'주요 노선 · 5문제',icon:'🌱',cls:'s1',color:'#4CAF50',qCount:5,passRate:.6,lines:['2','3','4']},
  {id:2,name:'숙련',desc:'혼합 출제 · 7문제',icon:'🚀',cls:'s2',color:'#2196F3',qCount:7,passRate:.65,lines:['1','2','3','4','5']},
  {id:3,name:'마스터',desc:'전 노선 · 10문제',icon:'⭐',cls:'s3',color:'#FF9800',qCount:10,passRate:.7,lines:['1','2','3','4','5','6','7','8','9']},
  {id:4,name:'도전',desc:'전 노선 · 10문제 (초성↑)',icon:'🔥',cls:'sb',color:'#E91E63',qCount:10,passRate:.7,lines:['1','2','3','4','5','6','7','8','9'],bonusStage:true},
];
const DAILY_STAGE={id:'daily',name:'데일리 챌린지',desc:'오늘의 5문제',color:'#7F77DD',qCount:5,passRate:.6,lines:['1','2','3','4','5','6','7','8','9'],isDaily:true};

// ── STATE ──
const S={
  clearedStages: JSON.parse(localStorage.getItem('cS')||'[]'),
  stageStars:    JSON.parse(localStorage.getItem('sS')||'{}'),
  totalScore:    parseInt(localStorage.getItem('tS')||'0'),
  dailyDate:     localStorage.getItem('dD')||'',
  dailyDone:     localStorage.getItem('dDone')==='1',
  dailyScore:    parseInt(localStorage.getItem('dScore')||'0'),
  hintCount:     parseInt(localStorage.getItem('hC')||'3'),
  hintDate:      localStorage.getItem('hDate')||'',
  // session
  currentStage:null,questions:[],qIndex:0,correct:0,score:0,combo:0,lives:3,answered:false,
};

function today(){ return new Date().toISOString().slice(0,10); }
function save(){
  localStorage.setItem('cS',JSON.stringify(S.clearedStages));
  localStorage.setItem('sS',JSON.stringify(S.stageStars));
  localStorage.setItem('tS',S.totalScore);
  localStorage.setItem('dD',S.dailyDate);
  localStorage.setItem('dDone',S.dailyDone?'1':'0');
  localStorage.setItem('dScore',S.dailyScore);
  localStorage.setItem('hC',S.hintCount);
  localStorage.setItem('hDate',S.hintDate);
}

// 매일 힌트 3개 리셋
function checkHintReset(){
  if(S.hintDate!==today()){S.hintCount=3;S.hintDate=today();save();}
}

// ── UTILS ──
function shuffle(a){return[...a].sort(()=>Math.random()-.5)}
function pick(a,n){return shuffle(a).slice(0,n)}

// seeded random (날짜 seed)
function seededRand(seed){
  let s=seed;
  return function(){s=(s*9301+49297)%233280;return s/233280;}
}
function seededShuffle(arr,rng){
  const a=[...arr];
  for(let i=a.length-1;i>0;i--){const j=Math.floor(rng()*(i+1));[a[i],a[j]]=[a[j],a[i]];}
  return a;
}

function getChosung(str){
  const CHO=['ㄱ','ㄲ','ㄴ','ㄷ','ㄸ','ㄹ','ㅁ','ㅂ','ㅃ','ㅅ','ㅆ','ㅇ','ㅈ','ㅉ','ㅊ','ㅋ','ㅌ','ㅍ','ㅎ'];
  return[...str].map(c=>{const code=c.charCodeAt(0)-0xAC00;if(code<0||code>11171)return c;return CHO[Math.floor(code/28/21)];}).join('');
}

// ── QUESTION GENERATOR ──
function generateQuestions(stage, dateStr){
  const pool=STATIONS.filter(s=>stage.lines.includes(s[0]));
  let selected;
  if(dateStr){
    // 날짜 seed로 항상 같은 문제 선택
    const seed=parseInt(dateStr.replace(/-/g,''))%233280;
    const rng=seededRand(seed);
    selected=seededShuffle(pool,rng).slice(0,stage.qCount);
  } else {
    selected=pick(pool,stage.qCount);
  }
  const chosungRatio=stage.bonusStage?.6:(stage.id===1?.2:.4);
  return selected.map(s=>{
    const useChosung=Math.random()<chosungRatio;
    if(useChosung){
      return{type:'B',line:s[0],station:s[1],chosung:getChosung(s[1])};
    } else {
      const answer=s[3];
      const wrongs=pick(pool.filter(x=>x[1]!==answer&&x[1]!==s[1]&&x[1]!==s[2]&&x[1]!==s[3]),3).map(x=>x[1]);
      return{type:'A',line:s[0],station:s[1],answer,options:shuffle([answer,...wrongs])};
    }
  });
}

// ── SCREENS ──
function showScreen(id){document.querySelectorAll('.screen').forEach(s=>s.classList.remove('active'));document.getElementById(id).classList.add('active');}

// ── HOME ──
function renderHome(){
  checkHintReset();
  document.getElementById('totalScore').textContent=S.totalScore.toLocaleString()+'점';

  // daily card
  const isDone=S.dailyDone&&S.dailyDate===today();
  document.getElementById('dailyCardWrap').innerHTML=`
    <div class="daily-card${isDone?' done':''}" onclick="${isDone?'':'startDaily()'}">
      <div class="dc-label">TODAY'S CHALLENGE</div>
      <div class="dc-title">📅 데일리 챌린지</div>
      <div class="dc-sub">${isDone?'오늘은 이미 도전했어요':'매일 새로운 5문제 · 오늘만 도전 가능'}</div>
      ${isDone?`<div class="dc-badge">✓ 완료 ${S.dailyScore.toLocaleString()}점</div>`:''}
      <div class="dc-hint-row">
        <div class="dc-hint-chip">💡 힌트 ${S.hintCount}개 남음</div>
        ${S.hintCount===0?'<div class="dc-hint-chip">광고 보고 충전</div>':''}
      </div>
    </div>`;

  // stage list
  const list=document.getElementById('stageList');
  list.innerHTML='';
  STAGES.forEach((stage,idx)=>{
    const unlocked=idx===0||S.clearedStages.includes(idx);
    const stars=S.stageStars[stage.id]||0;
    const locked=!unlocked;
    const card=document.createElement('div');
    card.className=`stage-card ${stage.cls}${locked?' locked':''}`;
    card.innerHTML=`
      <div class="sc-icon">${stage.icon}</div>
      <div class="sc-info">
        <div class="sc-name">Stage ${stage.id} · ${stage.name}</div>
        <div class="sc-desc">${stage.desc}</div>
      </div>
      <div>${locked?'🔒':`<span class="sc-stars">${'⭐'.repeat(stars)}${'☆'.repeat(3-stars)}</span>`}</div>`;
    if(!locked)card.onclick=()=>startStage(stage);
    list.appendChild(card);
  });
  showScreen('screenHome');
}

// ── START DAILY ──
function startDaily(){
  S.currentStage={...DAILY_STAGE};
  S.questions=generateQuestions(DAILY_STAGE, today());
  S.qIndex=0;S.correct=0;S.score=0;S.combo=0;S.lives=3;S.answered=false;
  document.getElementById('quizStageName').textContent='📅 데일리 챌린지';
  document.getElementById('quizStageDesc').textContent=today()+' · 5문제';
  document.getElementById('progFill').style.background=DAILY_STAGE.color;
  showScreen('screenQuiz');
  renderQuestion();
}

// ── START STAGE ──
function startStage(stage){
  S.currentStage=stage;
  S.questions=generateQuestions(stage);
  S.qIndex=0;S.correct=0;S.score=0;S.combo=0;S.lives=3;S.answered=false;
  document.getElementById('quizStageName').textContent=`Stage ${stage.id} · ${stage.name}`;
  document.getElementById('quizStageDesc').textContent=stage.desc;
  document.getElementById('progFill').style.background=stage.color;
  showScreen('screenQuiz');
  renderQuestion();
}

// ── RENDER QUESTION ──
function renderQuestion(){
  const q=S.questions[S.qIndex];
  const total=S.questions.length;
  S.answered=false;
  document.getElementById('progFill').style.width=(S.qIndex/total*100)+'%';
  document.getElementById('progText').textContent=`${S.qIndex+1}/${total}`;
  document.getElementById('progCorrect').textContent=`정답 ${S.correct}`;
  document.getElementById('quizScore').textContent=S.score.toLocaleString();
  document.getElementById('livesDisplay').innerHTML=Array.from({length:3},(_,i)=>`<span class="heart">${i<S.lives?'❤️':'🖤'}</span>`).join('');

  const line=LINES[q.line];
  const hintDisabled=S.hintCount<=0||q.type==='B';
  const body=document.getElementById('quizBody');

  const hintBar=`
    <div class="hint-bar">
      <span class="hint-count">💡 힌트 ${S.hintCount}개</span>
      <button class="hint-btn${hintDisabled?' disabled':''}" onclick="useHint()" id="hintBtn">
        💡 힌트 사용
      </button>
      ${S.hintCount===0?`<button class="hint-ad-btn" onclick="watchAd()">📺 광고 보고 충전</button>`:''}
    </div>`;

  if(q.type==='A'){
    body.innerHTML=`
      <div class="quiz-type-badge badge-a">🔵 다음 역 맞추기</div>
      <div class="line-indicator">
        <div class="line-dot" style="background:${line.color}">${q.line}</div>
        <div class="line-name">${line.name}</div>
      </div>
      <div class="question-card">
        <div class="q-label">다음 역은?</div>
        <div class="q-station">${q.station}</div>
        <div class="q-sub">이 역의 다음 역을 고르세요</div>
      </div>
      ${hintBar}
      <div class="options" id="options">
        ${q.options.map((opt,i)=>`
          <button class="opt-btn" onclick="answerA('${opt}',this)" data-val="${opt}">
            <div class="opt-num">${i+1}</div><span>${opt}</span>
          </button>`).join('')}
      </div>
      <div class="feedback" id="feedback"></div>`;
  } else {
    body.innerHTML=`
      <div class="quiz-type-badge badge-b">🟡 초성 퀴즈</div>
      <div class="line-indicator">
        <div class="line-dot" style="background:${line.color}">${q.line}</div>
        <div class="line-name">${line.name}</div>
      </div>
      <div class="question-card">
        <div class="q-label">이 역의 이름은?</div>
        <div class="q-station" style="font-size:15px;color:#888">${line.name} 소속 역</div>
      </div>
      <div class="chosung-box">
        <div class="chosung-text">${q.chosung}</div>
        <div class="chosung-hint">초성을 보고 역이름을 입력하세요</div>
      </div>
      <div class="chosung-input-wrap">
        <input class="chosung-input" id="chosungInput" placeholder="역이름 입력..." maxlength="10"
          onkeydown="if(event.key==='Enter')submitChosung()"/>
        <button class="submit-btn" id="submitBtn" onclick="submitChosung()">확인</button>
      </div>
      <div class="feedback" id="feedback"></div>`;
    setTimeout(()=>document.getElementById('chosungInput')?.focus(),100);
  }
}

// ── HINT ──
function useHint(){
  const q=S.questions[S.qIndex];
  if(S.hintCount<=0||S.answered||q.type==='B')return;
  const btns=[...document.querySelectorAll('.opt-btn:not(.eliminated)')];
  const wrongs=btns.filter(b=>b.dataset.val!==q.answer);
  if(wrongs.length===0)return;
  const toElim=pick(wrongs,Math.min(2,wrongs.length));
  toElim.forEach(b=>b.classList.add('eliminated'));
  S.hintCount--;
  save();
  document.getElementById('hintBtn').textContent=`💡 힌트 ${S.hintCount}개`;
  if(S.hintCount<=0){
    document.getElementById('hintBtn').classList.add('disabled');
  }
  showToast('오답 2개를 제거했어요!');
}

function watchAd(){
  // 실제 앱에서는 광고 SDK 호출
  showToast('📺 광고 시청 완료! 힌트 +2개');
  S.hintCount=Math.min(S.hintCount+2,5);
  save();
  renderQuestion(); // 힌트 버튼 갱신
}

// ── ANSWER ──
function answerA(val,btn){
  if(S.answered)return;
  S.answered=true;
  const q=S.questions[S.qIndex];
  const correct=val===q.answer;
  document.querySelectorAll('.opt-btn').forEach(b=>{
    b.onclick=null;
    if(b.dataset.val===q.answer)b.classList.add('correct');
    else if(b===btn&&!correct)b.classList.add('wrong');
  });
  handleResult(correct);
}

function submitChosung(){
  if(S.answered)return;
  const input=document.getElementById('chosungInput');
  const val=input.value.trim();
  if(!val)return;
  S.answered=true;
  const q=S.questions[S.qIndex];
  const correct=val===q.station;
  input.classList.add(correct?'correct':'wrong');
  input.disabled=true;
  document.getElementById('submitBtn').disabled=true;
  if(!correct)input.value=`${val} → 정답: ${q.station}`;
  handleResult(correct);
}

function handleResult(correct){
  const fb=document.getElementById('feedback');
  if(correct){
    S.correct++;S.combo++;
    const bonus=Math.min(S.combo*10,50);
    const gained=100+bonus;
    S.score+=gained;S.totalScore+=gained;
    save();
    fb.className='feedback correct';
    fb.textContent=S.combo>=2?`🔥 ${S.combo}콤보! +${gained}점`:`✅ 정답! +${gained}점`;
    if(S.combo>=2)showCombo(S.combo);
  } else {
    S.combo=0;S.lives--;
    fb.className='feedback wrong';
    fb.textContent='❌ 틀렸어요';
    document.getElementById('livesDisplay').innerHTML=Array.from({length:3},(_,i)=>`<span class="heart">${i<S.lives?'❤️':'🖤'}</span>`).join('');
  }
  document.getElementById('quizScore').textContent=S.score.toLocaleString();
  const delay=correct?900:1400;
  setTimeout(()=>{
    if(S.lives<=0){showResult();return;}
    S.qIndex+1>=S.questions.length?showResult():nextQuestion();
  },delay);
}

function nextQuestion(){S.qIndex++;renderQuestion();}

// ── RESULT ──
function showResult(){
  const stage=S.currentStage;
  const total=S.questions.length;
  const rate=S.correct/total;
  const passed=rate>=stage.passRate;
  let stars=0;
  if(rate>=1.0)stars=3;else if(rate>=.8)stars=2;else if(rate>=stage.passRate)stars=1;

  if(stage.isDaily){
    S.dailyDate=today();S.dailyDone=true;S.dailyScore=S.score;save();
  } else if(passed){
    if(!S.clearedStages.includes(stage.id))S.clearedStages.push(stage.id);
    if((S.stageStars[stage.id]||0)<stars)S.stageStars[stage.id]=stars;
    save();
  }

  const emoji=stars===3?'🏆':stars===2?'🎉':stars===1?'👍':'😢';
  const title=passed||stage.isDaily?(stage.isDaily?'오늘의 챌린지 완료!':'스테이지 클리어!'):'아쉽네요...';
  const sub=`${total}문제 중 ${S.correct}문제 정답`;

  document.getElementById('resultWrap').innerHTML=`
    <div class="result-emoji">${emoji}</div>
    ${stage.isDaily?'<div class="daily-result-badge">📅 데일리 챌린지</div>':''}
    <div class="result-title">${title}</div>
    <div class="result-sub">${sub}${!stage.isDaily&&passed?'\n다음 스테이지가 해금되었어요!':''}</div>
    <div class="result-score">${S.score.toLocaleString()}</div>
    <div class="result-score-label">이번 점수</div>
    <div class="stars-display">${'⭐'.repeat(stars)}${'☆'.repeat(3-stars)}</div>
    <div class="result-btns">
      ${stage.isDaily?'':`<button class="btn-primary" onclick="startStage(S.currentStage)">다시 도전</button>`}
      <button class="btn-secondary" onclick="renderHome()">홈으로</button>
    </div>`;
  showScreen('screenResult');
}

// ── COMBO / TOAST ──
function showCombo(n){
  const el=document.getElementById('comboBadge');
  el.textContent=`🔥 ${n}콤보!`;el.classList.add('show');
  setTimeout(()=>el.classList.remove('show'),1200);
}
function showToast(msg){
  const el=document.getElementById('toast');
  el.textContent=msg;el.classList.add('show');
  setTimeout(()=>el.classList.remove('show'),2000);
}

checkHintReset();
renderHome();
</script>
</body>
</html>
