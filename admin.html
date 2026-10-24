<!doctype html><html lang="ar" dir="rtl"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1"><title>مركز المشرف</title>
<style>
:root{--g:#0f9d6b;--gd:#0b4f3a;--gold:#d4a017;--bg:#f3f5f4;--c:#fff;--t:#16302a}
@media(prefers-color-scheme:dark){:root{--bg:#0e1a16;--c:#16251f;--t:#e6f2ed;--gd:#7fe0b9}}
*{box-sizing:border-box}body{margin:0;font-family:system-ui,sans-serif;background:var(--bg);color:var(--t);padding:14px;max-width:640px;margin:auto}
h1{color:var(--gd);font-size:20px}.u{background:var(--c);border-radius:14px;padding:14px;margin:10px 0;box-shadow:0 2px 10px #0001}
small{opacity:.65}.b{float:left;font-size:12px;padding:3px 9px;border-radius:20px;background:#8883}.published{background:var(--g);color:#fff}.approved{background:var(--gold);color:#fff}
button{font:inherit;border:0;border-radius:10px;padding:9px 12px;margin:6px 4px 0 0;background:var(--g);color:#fff}button.g{background:#8886}
.tabs button{background:var(--c);color:var(--t)}.tabs .on{background:var(--g);color:#fff}input{width:100%;padding:11px;margin:5px 0;border-radius:10px;border:1px solid #8884;font:inherit;background:var(--c);color:var(--t)}
li{padding:5px 0;cursor:pointer}ol{padding-right:22px;margin:8px 0 0}#msg{color:#c0392b;margin:8px 0}.hide{display:none}
</style></head><body>
<h1>🛠️ مركز المشرف — المنهج</h1><div id="msg"></div>
<div id="login" class="hide"><input id="em" type="email" placeholder="البريد"><input id="pw" type="password" placeholder="كلمة المرور"><button id="in">دخول</button></div>
<div id="main" class="hide"><div class="tabs"><button id="t1" class="on">الأول الثانوي</button><button id="t2">الثاني الثانوي</button></div>
<button id="imp" class="g">استيراد الفهرست كمسودة</button><button id="out" class="g">خروج</button>
<p><small>دورة النشر: مسودة ← مراجعة علمية ← معتمد ← منشور. اضغط على عنوان درس لتعديله.</small></p><div id="list"></div></div>
<script type="module">
import {firebaseConfig as cfg} from './firebase-config.js';
const A='https://www.gstatic.com/firebasejs/10.14.1/';
const [{initializeApp},au,fs]=await Promise.all(['firebase-app','firebase-auth','firebase-firestore'].map(m=>import(A+m+'.js')));
const app=initializeApp(cfg),auth=au.getAuth(app),db=fs.getFirestore(app);
const $=id=>document.getElementById(id),V='v2025',ST=['draft','review','approved','published'];
const LB={draft:'مسودة',review:'مراجعة علمية',approved:'معتمد',published:'منشور'};
const msg=t=>$('msg').textContent=t||'',esc=s=>String(s).replace(/[&<>"]/g,c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;'}[c]));
const col=n=>fs.collection(db,'curriculum_versions',V,n);
const S=[
[1,1,'مدخل إلى علم الأحياء','Introduction to Biology',5,[['مفهوم علم الأحياء',9],['علاقة علم الأحياء بالعلوم الأخرى',9],['أهمية علم الأحياء',10],['مجالات تطبيق علم الأحياء',10],['المستجدات العلمية في علم الأحياء',11],['فروع علم الأحياء',12],['خصائص الحياة',14],['مختبر الأحياء',16],['الطريقة العلمية',19],['الإحصاء الحيوي',24]]],
[1,2,'بيولوجية الخلية','Cell Biology',27,[['اكتشاف الخلية',28],['نظرية الخلية',30],['أجزاء الخلية',31],['تصنيف الخلايا',32],['تركيب خلايا حقيقية النواة',34],['التنظيم في الكائنات الحية',50],['دورة الخلية',53],['الانقسام الفتيلي',54],['الانقسام الاختزالي',58]]],
[1,3,'تصنيف الكائنات الحية','Taxonomy of Living Organisms',67,[['مقدمة',68],['التطور التاريخي لتصنيف الكائنات الحية',69],['التصنيف الجزيئي الحديث',70],['مستويات التصنيف',71],['التسمية العلمية',72],['مجال الأرشي بكتيريا',76],['عالم البكتيريا',78],['مملكة الطلائعيات',81],['مملكة الفطريات',85],['مملكة النباتات',87],['مملكة الحيوانات',95]]],
[1,4,'الدعامة في الكائنات الحية','Support in Living Organisms',105,[['أنواع الدعامة في الكائنات الحية',106],['الدعامة الهيدروستاتيكية في الأوليات',109],['الدعامة الهيدروستاتيكية في النباتات',113],['الدعامة الهيكلية الداخلية في النباتات',117],['الدعامة الهيكلية الخارجية في الحيوانات غير الفقارية',119],['الهيكل الدعامي في الحيوانات الفقارية والإنسان',121]]],
[1,5,'الوراثة','Genetics',129,[['مقدمة',130],['الوراثة المندلية',130],['الوراثة أحادية الهجين',133],['أنماط التوريث',137],['العلاقة بين الأليلات والجينات',141],['الوراثة ثنائية الهجين',143],['التزاوج الاختباري',145],['نظرية الصبغيات',146],['مفهوم الجينات',148],['مفهوم الكروموسومات',149],['الارتباط',154],['العبور',154],['التباين الوراثي',155]]],
[1,6,'علم البيئة','Ecology',159,[['البيئة',160],['النظام البيئي',161],['هرم الطاقة في النظام البيئي',162],['هرم الغذاء في النظام البيئي',163],['الإنتاجية البيئية',165],['الجماعات الأحيائية',167],['العلاقات البيئية بين الكائنات الحية',168],['المقاومة البيئية',173],['صفات وديناميكية الجماعة',176],['بيئة المجتمعات',177],['التعاقب البيئي',178],['التنوع الأحيائي',180],['تأثير الإنسان على البيئة',183],['التحديات البيئية المستقبلية',188],['التنمية البيئية المستدامة',189]]],
[2,1,'الحركة في الكائنات الحية','Movement in living organisms',6,[['الحركة في الكائنات الحية',7],['الحركة الجزيئية',8],['الحركة الظاهرية في النباتات',12],['الحركة في الكائنات الحية الأولية',18],['الحركة في الهيدرا',20],['الحركة في الديدان',22],['الحركة في الحشرات',24],['الحركة في الأسماك',26],['الحركة في البرمائيات',28],['الحركة في الطيور',30],['الحركة في الإنسان',33]]],
[2,2,'التغذية في الكائنات الحية','Nutrition in living organisms',42,[['مفهوم التغذية والغذاء',42],['المركبات الغذائية وأهميتها الحيوية',45],['التغذية في النباتات',49],['التغذية في الحيوانات',59],['الجهاز الهضمي في الإنسان',65],['صحة الجهاز الهضمي',72]]],
[2,3,'التنفس في الكائنات الحية','Respiration in living organisms',80,[['مفهوم التنفس في الكائنات الحية',81],['التنفس في النبات',84],['التنفس في الحيوانات',91],['التنفس في الإنسان',94]]],
[2,4,'الإخراج في الكائنات الحية','Excretion in living organisms',102,[['مفهوم الإخراج',103],['النتح في النباتات',107],['طرائق الإخراج في الحيوانات',112],['الإخراج في الإنسان',115],['جلد الإنسان',121]]],
[2,5,'النقل في الكائنات الحية','Transport in living organisms',129,[['النقل في النبات',130],['النقل والجهاز الدوري في الحيوانات',141],['الجهاز الدوري في الإنسان',147],['فصائل الدم',154]]],
[2,6,'الإحساس في الكائنات الحية','Sensation in living organisms',163,[['الإحساس في الكائنات الحية',164],['الإحساس في الحيوانات',169],['تركيب الجهاز الحسي في الإنسان',172]]],
[2,7,'التنظيم الهرموني في الكائنات الحية','Hormonal coordination in living organisms',193,[['التنظيم الهرموني في الكائنات الحية',194],['التنسيق الهرموني في الحيوانات',201],['التنسيق الهرموني في الإنسان',202]]]];
let U=[],L=[],grade=1;
const audit=(b,o)=>b.set(fs.doc(fs.collection(db,'audit_logs')),{...o,by:auth.currentUser.uid,at:fs.serverTimestamp()});
async function load(){try{const [u,l]=await Promise.all([fs.getDocs(col('units')),fs.getDocs(col('lessons'))]);
 U=u.docs.map(d=>({id:d.id,...d.data()}));L=l.docs.map(d=>({id:d.id,...d.data()}));render()}catch{msg('تعذر تحميل البيانات، تحقق من الاتصال.')}}
function render(){const us=U.filter(u=>u.gradeId==='secondary'+grade).sort((a,b)=>a.order-b.order);
 $('list').innerHTML=us.length?us.map(u=>{const ls=L.filter(l=>l.unitId===u.id).sort((a,b)=>a.order-b.order),i=ST.indexOf(u.status);
 return `<div class="u"><span class="b ${u.status}">${LB[u.status]}</span><b>${esc(u.title)}</b><br><small>${esc(u.titleEn)} · ص${u.page}</small>
 <div>${i<3?`<button data-s="${u.id}|${ST[i+1]}">إلى: ${LB[ST[i+1]]}</button>`:''}${i>0?`<button class="g" data-s="${u.id}|draft">إرجاع لمسودة</button>`:''}</div>
 <ol>${ls.map(l=>`<li data-e="${l.id}">${esc(l.title)} <small>ص${l.page}</small></li>`).join('')}</ol></div>`}).join(''):'<p>لا توجد بيانات بعد. اضغط «استيراد الفهرست».</p>'}
$('list').onclick=async e=>{msg();try{
 const s=e.target.closest('[data-s]'),t=e.target.closest('[data-e]');
 if(s){const [id,to]=s.dataset.s.split('|'),u=U.find(x=>x.id===id),b=fs.writeBatch(db);
  b.update(fs.doc(col('units'),id),{status:to});L.filter(l=>l.unitId===id).forEach(l=>b.update(fs.doc(col('lessons'),l.id),{status:to}));
  audit(b,{action:'unit_status',unit:id,from:u.status,to});await b.commit();await load()}
 else if(t){const l=L.find(x=>x.id===t.dataset.e),n=prompt('عنوان الدرس:',l.title);
  if(n&&n.trim()&&n.trim()!==l.title){const b=fs.writeBatch(db);b.update(fs.doc(col('lessons'),l.id),{title:n.trim()});
   audit(b,{action:'lesson_title',lesson:l.id,from:l.title,to:n.trim()});await b.commit();await load()}}
}catch{msg('فشلت العملية، تأكد من صلاحية المشرف والاتصال.')}};
$('imp').onclick=async()=>{if(U.length&&!confirm('توجد بيانات، وسيعاد تعيينها كمسودات وتُلغى تعديلاتك على العناوين. متابعة؟'))return;msg();
 try{let b=fs.writeBatch(db),n=0;const f=async()=>{await b.commit();b=fs.writeBatch(db);n=0};
 b.set(fs.doc(db,'curriculum_versions',V),{name:'الطبعة الأولى 2025 - المنهج السوداني',createdAt:fs.serverTimestamp()});n++;
 for(const [g,k,t,te,p,ls] of S){const uid=`g${g}u${k}`;
  b.set(fs.doc(col('units'),uid),{gradeId:'secondary'+g,order:k,title:t,titleEn:te,page:p,status:'draft'});n++;
  for(let i=0;i<ls.length;i++){b.set(fs.doc(col('lessons'),uid+'l'+String(i+1).padStart(2,'0')),{unitId:uid,gradeId:'secondary'+g,order:i+1,title:ls[i][0],page:ls[i][1],status:'draft'});if(++n>=400)await f()}}
 await b.commit();await load()}catch{msg('فشل الاستيراد، حاول مرة أخرى.')}};
const tab=g=>{grade=g;$('t1').classList.toggle('on',g==1);$('t2').classList.toggle('on',g==2);render()};
$('t1').onclick=()=>tab(1);$('t2').onclick=()=>tab(2);$('out').onclick=()=>au.signOut(auth);
$('in').onclick=async()=>{msg();try{await au.signInWithEmailAndPassword(auth,$('em').value.trim(),$('pw').value)}catch{msg('البريد أو كلمة المرور غير صحيحة.')}};
au.onAuthStateChanged(auth,async u=>{$('login').classList.toggle('hide',!!u);$('main').classList.add('hide');if(!u)return;
 try{const a=await fs.getDoc(fs.doc(db,'admins',u.uid));
  if(!a.exists()){msg('هذا الحساب ليس مشرفًا.');$('main').classList.remove('hide');$('list').innerHTML='';$('imp').classList.add('hide');return}
  $('imp').classList.remove('hide');$('main').classList.remove('hide');await load()}catch{msg('تعذر التحقق من الصلاحية.')}});
</script></body></html>
