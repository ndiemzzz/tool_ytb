<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Đọc kịch bản audio</title>
<style>
:root{box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px);
--bg:#f6f5f1;--card:#fff;--ink:#1d1d1b;--mute:#6f6e68;--line:#e2e0d8;--accent:#c2410c;--hl:#fff1e0;--dir:#7a6f9b}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#161615;--card:#201f1e;--ink:#f1efe8;--mute:#9b9a92;--line:#34332f;--accent:#fb923c;--hl:#3a2a1a;--dir:#a99bd0}}
:root[data-theme="dark"]{--bg:#161615;--card:#201f1e;--ink:#f1efe8;--mute:#9b9a92;--line:#34332f;--accent:#fb923c;--hl:#3a2a1a;--dir:#a99bd0}
*,*:before,*:after{box-sizing:inherit}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);color:var(--ink);font-family:system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;line-height:1.5}
.app{max-width:1100px;margin:0 auto;padding:16px;display:grid;gap:14px}
h1{font-size:20px;margin:0}
h2{font-size:15px;margin:0 0 8px}
.sub{color:var(--mute);font-size:13px;margin:2px 0 0}
.grid{display:grid;grid-template-columns:1fr 1.3fr;gap:14px}
@media(max-width:800px){.grid{grid-template-columns:1fr}}
.card{background:var(--card);border:1px solid var(--line);border-radius:14px;padding:14px}
textarea,input[type=text]{width:100%;border:1px solid var(--line);border-radius:10px;padding:10px;background:var(--bg);color:var(--ink);font:14px/1.5 inherit;font-family:inherit}
textarea{height:340px;resize:vertical}
label{font-size:12px;color:var(--mute);display:block;margin-bottom:3px}
.row{display:flex;flex-wrap:wrap;gap:12px;align-items:end;margin-top:10px}
.row>div{flex:1 1 130px;min-width:0}
select,input[type=range]{width:100%}
select{padding:7px;border-radius:8px;border:1px solid var(--line);background:var(--bg);color:var(--ink)}
button{cursor:pointer;border:1px solid var(--line);background:var(--card);color:var(--ink);padding:9px 14px;border-radius:10px;font-size:14px}
button:disabled{opacity:.5;cursor:default}
button.p{background:var(--accent);border-color:var(--accent);color:#fff;font-weight:600}
.seg{display:flex;gap:6px}
.seg button.on{background:var(--ink);color:var(--bg);border-color:var(--ink)}
#view{height:460px;overflow-y:auto;border-radius:10px;background:var(--bg);padding:40% 16px;position:relative;scroll-behavior:auto}
#inner.mirror{transform:scaleX(-1)}
.line{padding:8px 12px;border-radius:10px;margin:4px 0;cursor:pointer;opacity:.55;transition:opacity .2s,background .2s}
.line.cur{opacity:1;background:var(--hl);border-left:4px solid var(--accent)}
.line.dir{color:var(--dir);font-style:italic;font-size:.8em}
.who{display:inline-block;font-size:.55em;font-weight:700;letter-spacing:.04em;text-transform:uppercase;color:var(--accent);margin-right:8px;vertical-align:middle}
#cd{position:absolute;inset:0;display:none;align-items:center;justify-content:center;font-size:96px;font-weight:700;color:var(--accent);background:color-mix(in srgb,var(--bg) 85%,transparent);z-index:2}
.bar{display:flex;gap:8px;flex-wrap:wrap;align-items:center;margin-bottom:10px}
.note{font-size:12px;color:var(--mute);margin-top:8px}
.prog{height:4px;background:var(--line);border-radius:4px;margin-top:10px;overflow:hidden}
.prog i{display:block;height:100%;width:0;background:var(--accent)}
.chk{display:flex;gap:6px;align-items:center;font-size:13px;color:var(--ink);margin:0}
</style>
</head>
<body>
<div class="app">
  <div><h1>🎙️ Đọc kịch bản audio</h1>
  <p class="sub">Tạo nội dung bằng AI, rồi cho máy đọc, tự đọc theo teleprompter hoặc xuất MP3.</p></div>

  <div class="card" id="genCard">
    <h2>✨ Tự tạo nội dung</h2>
    <label for="topic">Chủ đề / ý chính</label>
    <input type="text" id="topic" placeholder="VD: 5 thói quen buổi sáng giúp tập trung hơn">
    <div class="row">
      <div><label>Thể loại</label><select id="gtype">
        <option value="podcast đối thoại giữa người dẫn và khách mời">Podcast đối thoại</option>
        <option value="truyện kể / audio story có người kể chuyện và nhân vật">Kể chuyện</option>
        <option value="kịch bản video YouTube một người dẫn">Video một người dẫn</option>
        <option value="quảng cáo / bản tin ngắn hấp dẫn">Quảng cáo, bản tin</option>
        <option value="bài thuyết trình, diễn thuyết">Thuyết trình</option>
      </select></div>
      <div><label>Độ dài</label><select id="glen">
        <option value="150">Ngắn (~1 phút)</option>
        <option value="450" selected>Vừa (~3 phút)</option>
        <option value="900">Dài (~6 phút)</option>
        <option value="3000">Rất dài (~20 phút)</option>
        <option value="3750">Rất dài (~25 phút)</option>
        <option value="4500">Rất dài (~30 phút)</option>
      </select></div>
      <div><label>Giọng điệu</label><select id="gtone">
        <option>thân mật, tự nhiên</option><option>chuyên nghiệp, rõ ràng</option><option>hài hước, vui nhộn</option><option>truyền cảm, sâu lắng</option>
      </select></div>
      <div style="flex:0 0 auto"><button class="p" id="gen">✨ Tạo kịch bản</button> <button id="gstop" style="display:none">■ Hủy</button></div>
    </div>
    <div class="row" style="margin-top:6px"><div style="flex-basis:100%"><label class="chk"><input type="checkbox" id="autoexp"> Tự động xuất MP3 ngay sau khi tạo xong</label></div></div>
    <p class="note" id="gst"></p>
  </div>

  <div class="grid">
    <div class="card">
      <label for="src">Kịch bản (có thể chỉnh sửa)</label>
      <textarea id="src" spellcheck="false"></textarea>
      <p class="note">Mỗi dòng là một câu. Dùng <b>Tên: lời thoại</b> cho nhân vật, và <b>[ghi chú]</b> hoặc <b>(ghi chú)</b> cho hướng dẫn (không đọc).</p>
    </div>
    <div class="card">
      <div class="bar">
        <div class="seg" id="modes">
          <button data-m="tts" class="on">🔊 Máy đọc</button>
          <button data-m="tele">📜 Teleprompter</button>
        </div>
        <button class="p" id="play">▶ Bắt đầu</button>
        <button id="stop">■ Dừng</button>
        <button id="exp">⬇ Xuất MP3</button>
      </div>
      <p class="note" id="st" style="margin:0 0 8px;color:var(--accent)"></p><textarea id="code" readonly onclick="this.select()" style="display:none;height:150px;margin-bottom:8px"></textarea>
      <div class="prog"><i id="pg"></i></div>
      <div id="view" style="margin-top:10px"><div id="cd"></div><div id="inner"></div></div>
      <div class="row">
        <div><label>Tốc độ: <span id="spv"></span></label><input type="range" id="sp" min="1" max="10" value="4"></div>
        <div><label>Ngắt nghỉ giữa câu: <span id="pzv"></span>s</label><input type="range" id="pz" min="0" max="20" value="4"></div>
        <div><label>Cỡ chữ: <span id="fsv"></span>px</label><input type="range" id="fs" min="16" max="64" value="26"></div>
        <div id="vbox"><label>Giọng dự phòng (khi thiếu giọng)</label><select id="voice"></select></div>
        <div><label><input type="checkbox" id="mirror"> Lật gương</label></div>
        <div style="flex-basis:100%"><label>Giọng từng nhân vật khi xuất MP3</label><div id="spk"></div></div>
      </div>
      <p class="note" id="vn"></p>
    </div>
  </div>
</div>
<script>
const $=id=>document.getElementById(id);
const SAMPLE=`[Nhạc nền nhẹ, nhỏ dần]
Dẫn: Chào mừng các bạn đến với podcast Chuyện Đêm Khuya.
Dẫn: Hôm nay chúng ta sẽ nói về một chủ đề rất thú vị.
(ngừng 2 giây)
Khách: Cảm ơn bạn đã mời mình. Mình rất vui khi được ở đây.
Dẫn: Vậy hãy bắt đầu nhé!`;
let lines=[],cur=-1,playing=false,mode='tts',token=0,raf=null,voices=[];

function parse(){
  lines=$('src').value.split('\n').map(s=>s.trim()).filter(Boolean).map(r=>{
    if(/^[\[\(].*[\]\)]$/.test(r))return{type:'dir',text:r};
    const m=r.match(/^([^:：\[\(]{1,30})[:：]\s*(.+)$/);
    return m?{type:'say',who:m[1],text:m[2]}:{type:'say',who:'',text:r};
  });
}
function render(){
  const box=$('inner');box.textContent='';
  lines.forEach((l,i)=>{
    const d=document.createElement('div');d.className='line'+(l.type==='dir'?' dir':'');
    if(l.who){const w=document.createElement('span');w.className='who';w.textContent=l.who;d.appendChild(w)}
    d.appendChild(document.createTextNode(l.text));
    d.onclick=()=>{cur=i;mark();if(playing&&mode==='tts'){speak(i)}};
    box.appendChild(d);
  });
  mark();
}
const PRESETS={
hm:{n:'Nữ chuẩn (HoaiMy)',v:'vi-VN-HoaiMyNeural',r:0,p:0},
hy:{n:'Nữ trẻ, tươi sáng',v:'vi-VN-HoaiMyNeural',r:8,p:15},
hd:{n:'Nữ kể chuyện, dịu',v:'vi-VN-HoaiMyNeural',r:-10,p:-6},
nm:{n:'Nam chuẩn (NamMinh)',v:'vi-VN-NamMinhNeural',r:0,p:0},
nt:{n:'Nam trầm, ấm',v:'vi-VN-NamMinhNeural',r:-8,p:-15},
nn:{n:'Nam năng động',v:'vi-VN-NamMinhNeural',r:10,p:8},
ma:{n:'Đa ngôn ngữ nữ - Ava (thử nghiệm)',v:'en-US-AvaMultilingualNeural',r:0,p:0},
me:{n:'Đa ngôn ngữ nữ - Emma (thử nghiệm)',v:'en-US-EmmaMultilingualNeural',r:0,p:0},
mb:{n:'Đa ngôn ngữ nam - Andrew (thử nghiệm)',v:'en-US-AndrewMultilingualNeural',r:0,p:0},
mr:{n:'Đa ngôn ngữ nam - Brian (thử nghiệm)',v:'en-US-BrianMultilingualNeural',r:0,p:0}};
const PK=Object.keys(PRESETS),assign={};
function buildSpk(){
  const box=$('spk');box.textContent='';
  [...new Set(lines.filter(l=>l.type==='say').map(l=>l.who))].forEach((w,i)=>{
    if(!assign[w]||!PRESETS[assign[w]])assign[w]=['hm','nm','hy','nt','hd','nn'][i%6];
    const row=document.createElement('div');row.style.cssText='display:flex;gap:8px;align-items:center;margin-bottom:6px';
    const nm=document.createElement('span');nm.style.cssText='flex:0 0 90px;font-size:13px;font-weight:600';nm.textContent=w||'Người dẫn';
    const s=document.createElement('select');s.style.flex='1';
    PK.forEach(k=>{const o=document.createElement('option');o.value=k;o.textContent=PRESETS[k].n;s.appendChild(o)});
    s.value=assign[w];s.onchange=()=>{assign[w]=s.value};
    row.append(nm,s);box.appendChild(row);
  });
}
function mark(){
  [...$('inner').children].forEach((el,i)=>el.classList.toggle('cur',i===cur));
  $('pg').style.width=lines.length?Math.max(0,(cur+1)/lines.length*100)+'%':'0';
}
function centerOn(i){
  const el=$('inner').children[i],v=$('view');if(!el)return;
  v.scrollTo({top:el.offsetTop-v.clientHeight/2+el.clientHeight/2,behavior:'smooth'});
}
function pickVoice(pr){
  const k=(pr.v.match(/HoaiMy|NamMinh|Ava|Emma|Andrew|Brian/)||[''])[0];
  const m=voices.filter(v=>k&&v.name.includes(k));
  return m.find(x=>/online|natural/i.test(x.name))||m[0]||null;
}
function speak(i){
  token++;const my=token;speechSynthesis.cancel();
  while(i<lines.length&&lines[i].type==='dir')i++;
  if(i>=lines.length){stop(true);return}
  cur=i;mark();centerOn(i);
  const u=new SpeechSynthesisUtterance(lines[i].text);
  const pr=PRESETS[assign[lines[i].who]]||PRESETS.hm;
  const v=pickVoice(pr)||voices[$('voice').value];if(v){u.voice=v;u.lang=v.lang}else u.lang='vi-VN';
  u.rate=Math.min(10,Math.max(0.1,1+($('sp').value*10-40+pr.r)/100));u.pitch=Math.min(2,Math.max(0,1+pr.p/200));
  u.onend=()=>{setTimeout(()=>{if(playing&&my===token)speak(i+1)},$('pz').value*100)};
  u.onerror=()=>{if(playing&&my===token)speak(i+1)};
  speechSynthesis.speak(u);
}
function teleLoop(t){
  if(!playing||mode!=='tele')return;
  const v=$('view'),dt=(t-lastT)/1000;lastT=t;
  v.scrollTop+=$('sp').value*12*dt;
  const mid=v.scrollTop+v.clientHeight*0.5;
  [...$('inner').children].forEach((el,i)=>{if(el.offsetTop<=mid&&el.offsetTop+el.offsetHeight>mid&&cur!==i){cur=i;mark()}});
  if(v.scrollTop+v.clientHeight>=v.scrollHeight-2){stop(true);return}
  raf=requestAnimationFrame(teleLoop);
}
let lastT=0;
function start(){
  if(!lines.length)return;
  playing=true;$('play').textContent='⏸ Tạm dừng';
  if(mode==='tts'){
    const miss=[...new Set(lines.filter(l=>l.type==='say').map(l=>PRESETS[assign[l.who]]||PRESETS.hm))].filter(p=>!pickVoice(p)).map(p=>p.n);
    $('st').textContent=miss.length?'Trình duyệt này không có giọng: '+miss.join(', ')+'. Đang dùng giọng dự phòng nên nghe sẽ khác bản MP3. Hãy mở bằng Microsoft Edge.':'';
    speak(cur<0?0:cur)}
  else{
    const cd=$('cd');let n=3;cd.style.display='flex';cd.textContent=n;
    const tk=setInterval(()=>{
      if(!playing){clearInterval(tk);cd.style.display='none';return}
      n--;if(n>0){cd.textContent=n;return}
      clearInterval(tk);cd.style.display='none';
      lastT=performance.now();raf=requestAnimationFrame(teleLoop);
    },1000);
  }
}
function pause(){playing=false;token++;speechSynthesis.cancel();cancelAnimationFrame(raf);$('cd').style.display='none';$('play').textContent='▶ Tiếp tục'}
function stop(done){
  playing=false;token++;speechSynthesis.cancel();cancelAnimationFrame(raf);$('cd').style.display='none';
  $('play').textContent='▶ Bắt đầu';cur=-1;mark();$('view').scrollTo({top:0});
}
$('play').onclick=()=>playing?pause():start();
$('stop').onclick=()=>stop();

/* ---------- Xuất MP3 (tạo file chạy cục bộ dùng edge-tts) ---------- */
async function doExport(){
  const dl=window.claude?await claude.use('downloads'):null;
  const items=lines.filter(l=>l.type==='say').map(l=>[l.who,l.text]);
  if(!items.length){$('st').textContent='Chưa có lời thoại để xuất.';return}
  const base=$('sp').value*10-40,sg=n=>(n>=0?'+':'')+n,cfg={};
  [...new Set(items.map(x=>x[0]))].forEach(w=>{const p=PRESETS[assign[w]]||PRESETS.hm;cfg[w]=[p.v,sg(Math.round(base+p.r))+'%',sg(p.p)+'Hz']});
  let txt='';const fb=m=>{$('st').textContent=m;$('code').value=txt;$('code').style.display='block'};
  const L=['# Doi duoi .txt thanh .py roi chay: python chay-kich-ban.py','import asyncio, sys, subprocess','from pathlib import Path','try:','    import edge_tts','except ImportError:','    subprocess.check_call([sys.executable, "-m", "pip", "install", "edge-tts"])','    import edge_tts','ITEMS = '+JSON.stringify(items),'CFG = '+JSON.stringify(cfg),'PAUSE = '+($('pz').value/10),'SIL = bytes([255, 243, 100, 192]) + bytes(140)','async def say(line, v, r, p, tmp):','    for a in ((v, r, p), (v, r, p), (v, r, "+0Hz"), (v, "+0%", "+0Hz"), ("vi-VN-HoaiMyNeural", "+0%", "+0Hz")):','        try:','            await edge_tts.Communicate(line, a[0], rate=a[1], pitch=a[2]).save(str(tmp))','            await asyncio.sleep(0.3)','            return','        except edge_tts.exceptions.NoAudioReceived:','            print("  thu lai voi tham so khac:", a)','            await asyncio.sleep(2)','    raise SystemExit("Khong nhan duoc audio. Hay chay: pip install -U edge-tts")','async def main():','    data = []','    for i, (who, line) in enumerate(ITEMS, 1):','        v, r, p = CFG[who]','        tmp = Path(__file__).with_name("_part.mp3")','        await say(line, v, r, p, tmp)','        data.append(tmp.read_bytes()); tmp.unlink()','        data.append(SIL * round(PAUSE / 0.024))','        print(f"[{i}/{len(ITEMS)}] {line[:50]}")','    out = Path(__file__).with_name("kich-ban.mp3")','    out.write_bytes(b"".join(data))','    print("Xong:", out)','asyncio.run(main())','input("Nhan Enter de dong...")'];
  try{
    txt=L.join('\n');if(!dl)throw{code:'unavailable'};await dl.save({filename:'chay-kich-ban.txt',data:txt});
    $('st').textContent='Đã tải. Đổi đuôi .txt thành .py rồi chạy: python chay-kich-ban.py. File kich-ban.mp3 sẽ xuất hiện cùng thư mục (cần cài Python).';
  }catch(e){if(e&&e.code==='declined'){$('st').textContent='Bạn đã từ chối tải file.';return}fb('Không tải được file ('+((e&&(e.code||e.message))||'lỗi')+'). Hãy sao chép mã bên dưới, lưu thành chay-kich-ban.py rồi chạy.')}
}
$('exp').onclick=doExport;

/* ---------- Tự tạo nội dung bằng AI ---------- */
let genCtl=null;
function cleanScript(t){
  return t.replace(/```[a-z]*/gi,'').replace(/\*\*|__/g,'').replace(/^\s*#+\s*/gm,'').replace(/^\s*[-*•]\s+/gm,'').replace(/\n{2,}/g,'\n').trim();
}
async function generate(){
  const topic=$('topic').value.trim();
  if(!topic){$('gst').textContent='Hãy nhập chủ đề trước.';$('topic').focus();return}
  const sample=window.claude?await claude.use('sample'):null;
  if(!sample){$('gst').textContent='Tính năng tạo nội dung chỉ hoạt động khi mở trang này trên claude.ai (bản đã xuất bản).';return}
  stop();
  const words=$('glen').value;
  const prompt=`Hãy viết một kịch bản audio bằng tiếng Việt.
Thể loại: ${$('gtype').value}.
Chủ đề: ${topic}.
Giọng điệu: ${$('gtone').value}.
Độ dài: khoảng ${words} từ lời thoại.

QUY TẮC ĐỊNH DẠNG (bắt buộc, vì kịch bản sẽ được máy đọc thành giọng nói):
- Mỗi dòng là một câu hoặc một ý ngắn (tối đa khoảng 30 từ).
- Lời thoại viết theo dạng "Tên: lời thoại", tên nhân vật ngắn gọn (1-2 từ, không có dấu hai chấm), dùng nhất quán. Thể loại một người dẫn thì dùng một tên duy nhất, ví dụ "Dẫn".
- Hướng dẫn không đọc đặt trong [ngoặc vuông] trên dòng riêng, dùng rất ít.
- Viết số, ký hiệu, từ viết tắt thành chữ để đọc tự nhiên.
- Chỉ trả về kịch bản, không tiêu đề, không markdown, không giải thích, không đánh số.`;
  genCtl=new AbortController();
  $('gen').disabled=true;$('gstop').style.display='';$('gst').textContent='Đang tạo kịch bản…';
  try{
    if(Number(words)>900){await genLong(sample,topic,Number(words))}
    else{
      const r=await sample(prompt,{signal:genCtl.signal,cache:false,onText:({text})=>{$('src').value=cleanScript(text);$('src').scrollTop=1e9}});
      $('src').value=cleanScript(r.text||$('src').value);
    }
    $('src').dispatchEvent(new Event('input'));
    $('gst').textContent='Đã tạo xong. Bạn có thể chỉnh sửa, chọn giọng cho từng nhân vật rồi nghe thử hoặc xuất MP3.';
    if($('autoexp').checked)await doExport();
  }catch(e){
    if(genCtl&&genCtl.signal.aborted){$('src').dispatchEvent(new Event('input'));$('gst').textContent='Đã hủy.'}
    else if(e&&e.code==='not_granted')$('gst').textContent='Bạn chưa cấp quyền cho tính năng tạo nội dung.';
    else if(e&&e.code==='rate_limited')$('gst').textContent='Đang bị giới hạn lượt, hãy thử lại sau ít phút.';
    else $('gst').textContent='Không tạo được nội dung ('+((e&&(e.message||e.code))||'lỗi')+').';
  }finally{$('gen').disabled=false;$('gstop').style.display='none';genCtl=null}
}
/* Kịch bản dài 20-30 phút: lập dàn ý rồi viết từng phần nối tiếp nhau */
async function genLong(sample,topic,words){
  const sig=genCtl.signal,n=Math.ceil(words/700);
  const base=`Thể loại: ${$('gtype').value}. Chủ đề: ${topic}. Giọng điệu: ${$('gtone').value}.`;
  const RULES=`QUY TẮC: mỗi dòng là một câu hoặc ý ngắn (tối đa khoảng 30 từ). Lời thoại dạng "Tên: lời thoại", tên ngắn 1-2 từ, không có dấu hai chấm. Hướng dẫn không đọc đặt trong [ngoặc vuông] trên dòng riêng, dùng rất ít. Viết số và ký hiệu thành chữ. Chỉ trả về kịch bản, không tiêu đề, không markdown, không giải thích, không đánh số.`;
  $('gst').textContent='Đang lập dàn ý…';
  const o=await sample(`Lập dàn ý đúng ${n} phần cho một kịch bản audio tiếng Việt dài khoảng ${Math.round(words/150)} phút.\n${base}\nMỗi phần một dòng, dạng "Tên phần: nội dung chính (1-2 câu)". Chỉ trả về ${n} dòng, không đánh số, không markdown.`,{signal:sig,cache:false});
  const outline=cleanScript(o.text).split('\n').filter(Boolean).slice(0,n);
  const per=Math.round(words/outline.length);
  let script='';
  for(let i=0;i<outline.length;i++){
    $('gst').textContent=`Đang viết phần ${i+1}/${outline.length}… (có thể mất vài phút, đừng đóng trang)`;
    const names=[...new Set(script.split('\n').map(s=>(s.match(/^([^:：\[\(]{1,30})[:：]/)||[])[1]).filter(Boolean))];
    const p=`Bạn đang viết từng phần của một kịch bản audio tiếng Việt dài.\n${base}\nDÀN Ý CẢ KỊCH BẢN:\n${outline.map((s,k)=>(k+1)+'. '+s).join('\n')}\n\n${names.length?'Các nhân vật đã dùng (giữ nguyên tên): '+names.join(', ')+'.\n':''}${script?'Những dòng cuối của phần trước:\n'+script.split('\n').slice(-8).join('\n')+'\n':''}\nHãy viết PHẦN ${i+1}/${outline.length}: "${outline[i]}", khoảng ${per} từ lời thoại. ${i===0?'Đây là phần mở đầu, hãy chào và giới thiệu hấp dẫn.':'Viết nối tiếp tự nhiên, không chào lại, không lặp ý phần trước.'} ${i===outline.length-1?'Đây là phần cuối: tổng kết và kết thúc trọn vẹn.':'Chưa kết thúc cả kịch bản, không chào tạm biệt.'}\n${RULES}`;
    const r=await sample(p,{signal:sig,cache:false,onText:({text})=>{$('src').value=cleanScript(script+'\n'+text);$('src').scrollTop=1e9}});
    script=cleanScript(script+'\n'+r.text);
    $('src').value=script;
  }
}
$('gen').onclick=generate;
$('gstop').onclick=()=>{if(genCtl)genCtl.abort()};
$('topic').addEventListener('keydown',e=>{if(e.key==='Enter')generate()});

$('modes').onclick=e=>{
  const b=e.target.closest('button');if(!b)return;
  stop();mode=b.dataset.m;
  [...$('modes').children].forEach(x=>x.classList.toggle('on',x===b));
  $('vbox').style.display=mode==='tts'?'':'none';
  updLabels();
};
function updLabels(){
  $('spv').textContent=mode==='tts'?(0.6+$('sp').value*0.1).toFixed(1)+'x':$('sp').value*12+' px/s';
  $('fsv').textContent=$('fs').value;
  $('inner').style.fontSize=$('fs').value+'px';
  $('inner').classList.toggle('mirror',$('mirror').checked);
}
$('pz').addEventListener('input',()=>{$('pzv').textContent=($('pz').value/10).toFixed(1)});$('pzv').textContent='0.4';
['sp','fs','mirror'].forEach(id=>$(id).addEventListener('input',updLabels));
$('sp').addEventListener('change',()=>{if(playing&&mode==='tts')speak(cur)});
let tm;$('src').addEventListener('input',()=>{
  stop();parse();render();buildSpk();
  clearTimeout(tm);tm=setTimeout(()=>{try{localStorage.setItem('script_v1',$('src').value)}catch(e){}},400);
});
function loadVoices(){
  const sc=v=>(/^vi/i.test(v.lang)?10:0)+(/natural|online|neural/i.test(v.name)?5:0)+(/google/i.test(v.name)?2:0);
  voices=speechSynthesis.getVoices().slice().sort((a,b)=>sc(b)-sc(a));
  const sel=$('voice');sel.textContent='';
  voices.forEach((v,i)=>{const o=document.createElement('option');o.value=i;o.textContent=(/natural|online|neural/i.test(v.name)?'⭐ ':'')+v.name+' ('+v.lang+')';sel.appendChild(o)});
  const vi=voices.findIndex(v=>/^vi/i.test(v.lang));
  if(vi>=0)sel.value=vi;
  const nat=voices.some(v=>/^vi/i.test(v.lang)&&/natural|online|neural/i.test(v.name));
  $('vn').textContent=nat?'Đang dùng giọng neural tự nhiên (⭐).':'Chưa có giọng tiếng Việt tự nhiên. Mở trang này bằng Microsoft Edge để có giọng "Microsoft HoaiMy / NamMinh Online (Natural)" giống giọng YouTube.';
}
if('speechSynthesis' in window){loadVoices();speechSynthesis.onvoiceschanged=loadVoices}
else{$('vn').textContent='Trình duyệt không hỗ trợ đọc giọng nói. Hãy dùng Teleprompter.'}
let saved=null;try{saved=localStorage.getItem('script_v1')}catch(e){}
$('src').value=saved||SAMPLE;
parse();render();updLabels();buildSpk();
</script>
</body>
</html>
