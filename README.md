<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
<title>Nosso Guia Disney</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&family=Nunito:ital,wght@0,400;0,600;0,700;0,800;1,600&display=swap" rel="stylesheet">
<script>
/*__DATA_START__*/
window.EMBEDDED_DATA = {"checks":{"d1_3":1,"d1_4":1,"d1_5":1,"d1_6":1,"d1_7":1,"d1_8":1,"d1_9":1}};
/*__DATA_END__*/
</script>
<script defer src="https://cdn.jsdelivr.net/npm/heic2any@0.0.4/dist/heic2any.min.js" onerror="window.__noHeic=true"></script>
<style>
  :root{
    --night:#15102e; --night2:#1f1745; --panel:#241a52; --panel2:#2c2161;
    --gold:#ffce5c; --gold-soft:#ffe39b; --magenta:#ff6fb5; --cyan:#62e6ff;
    --text:#f4f0ff; --muted:#b9aee6;
    --green:#5fe089; --yellow:#ffd24a; --red:#ff7a7a; --line:rgba(255,255,255,.10);
    --warm1:#3a2330; --warm2:#2a1830; --warmgold:#ffd9a0; --rose:#ff9ec4;
  }
  *{box-sizing:border-box;margin:0;padding:0;-webkit-tap-highlight-color:transparent;}
  body{font-family:'Nunito',sans-serif;
    background:radial-gradient(1200px 600px at 50% -10%, #3a2a78 0%, transparent 55%),radial-gradient(800px 500px at 90% 20%, rgba(255,111,181,.12) 0%, transparent 50%),linear-gradient(180deg, var(--night2) 0%, var(--night) 100%);
    background-attachment:fixed;color:var(--text);line-height:1.5;padding-bottom:90px;min-height:100vh;overflow-x:hidden;transition:background .6s ease;}
  body.warm{background:radial-gradient(1000px 600px at 50% -10%, #6b3a4a 0%, transparent 55%),radial-gradient(700px 500px at 85% 25%, rgba(255,158,196,.16) 0%, transparent 55%),linear-gradient(180deg, var(--warm1) 0%, var(--warm2) 100%);}
  .stars,.stars2{position:fixed;inset:0;pointer-events:none;z-index:0;}
  .stars{opacity:.6;animation:tw 4s ease-in-out infinite;background-image:radial-gradient(1.5px 1.5px at 20% 30%, #fff, transparent),radial-gradient(1.5px 1.5px at 70% 15%, #fff, transparent),radial-gradient(1px 1px at 40% 60%, #fff, transparent),radial-gradient(1.5px 1.5px at 15% 80%, #fff, transparent),radial-gradient(1px 1px at 90% 70%, #fff, transparent);}
  .stars2{opacity:.4;animation:tw 6s ease-in-out infinite 1s;background-image:radial-gradient(1px 1px at 55% 25%, var(--gold-soft), transparent),radial-gradient(1px 1px at 30% 45%, #fff, transparent),radial-gradient(1.5px 1.5px at 80% 50%, var(--cyan), transparent),radial-gradient(1px 1px at 60% 85%, #fff, transparent);}
  @keyframes tw{0%,100%{opacity:.25}50%{opacity:.7}}
  .wrap{position:relative;z-index:1;max-width:560px;margin:0 auto;padding:0 16px;}

  .splash{position:fixed;inset:0;z-index:80;display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center;padding:30px;overflow:auto;
    background:radial-gradient(900px 500px at 50% 10%, #4a2f8f 0%, transparent 60%),linear-gradient(180deg,#241a52,#15102e);animation:fadein .5s ease;}
  .splash.hide{display:none;}
  .splash-corner{position:absolute;top:14px;background:rgba(255,255,255,.08);border:1px solid var(--line);color:var(--gold-soft);font-family:'Fredoka',sans-serif;font-weight:600;font-size:13px;padding:8px 13px;border-radius:999px;cursor:pointer;}
  .splash-corner.left{left:14px;}
  .splash-corner.right{right:14px;}
  .splash .scastle{font-size:64px;animation:float 4s ease-in-out infinite;filter:drop-shadow(0 6px 30px rgba(255,206,92,.55));}
  .splash h1{font-family:'Fredoka',sans-serif;font-weight:700;font-size:30px;margin-top:8px;background:linear-gradient(95deg,var(--gold-soft),var(--gold),var(--magenta),var(--cyan));background-size:200% auto;-webkit-background-clip:text;background-clip:text;-webkit-text-fill-color:transparent;animation:shine 6s linear infinite;}
  .splash .sub{color:var(--muted);font-size:14.5px;margin-top:8px;max-width:320px;}
  .splash .who-q{color:var(--gold-soft);font-weight:800;font-size:13px;margin-top:24px;margin-bottom:12px;}
  .avatars{display:flex;gap:10px;justify-content:flex-start;flex-wrap:nowrap;overflow-x:auto;max-width:100%;padding:4px 2px;-webkit-overflow-scrolling:touch;}
  .avatar{flex:0 0 auto;}
  .avatar{display:flex;flex-direction:column;align-items:center;gap:6px;cursor:pointer;position:relative;}
  .aimg{width:60px;height:60px;border-radius:50%;background:rgba(255,255,255,.08);border:2px solid var(--line);display:flex;align-items:center;justify-content:center;font-family:'Fredoka',sans-serif;font-size:24px;font-weight:700;color:var(--gold-soft);overflow:hidden;transition:all .2s;}
  .aimg img{width:100%;height:100%;object-fit:cover;}
  .avatar.sel .aimg{border-color:var(--gold);box-shadow:0 0 18px rgba(255,206,92,.5);transform:scale(1.06);}
  .avatar span{font-family:'Fredoka',sans-serif;font-weight:600;font-size:13px;color:var(--text);}
  .acam{position:absolute;top:-4px;right:2px;width:22px;height:22px;border-radius:50%;background:var(--magenta);color:#fff;display:flex;align-items:center;justify-content:center;font-size:12px;cursor:pointer;border:2px solid #241a52;}
  .acam input{display:none;}
  #guestName{width:100%;max-width:260px;text-align:center;background:rgba(0,0,0,.3);border:1px solid var(--line);border-radius:14px;padding:12px;color:var(--text);font-family:'Fredoka',sans-serif;font-size:16px;margin-top:16px;}
  #guestName::placeholder{color:var(--muted);}
  .paths{display:none;flex-direction:column;gap:12px;width:100%;max-width:300px;margin-top:22px;}
  .paths.show{display:flex;animation:rise .4s ease;}
  .pbtn{font-family:'Fredoka',sans-serif;font-weight:600;font-size:16px;padding:15px;border-radius:16px;border:none;cursor:pointer;transition:transform .15s;display:flex;align-items:center;justify-content:center;gap:9px;}
  .pbtn:active{transform:scale(.97);}
  .pbtn.guide{background:linear-gradient(135deg,var(--cyan),#3aa6c9);color:#06222b;box-shadow:0 8px 22px rgba(98,230,255,.3);}
  .pbtn.mem{background:linear-gradient(135deg,var(--magenta),#c44ea0);color:#fff;box-shadow:0 8px 22px rgba(255,111,181,.35);}
  .splash .tip{color:var(--muted);font-size:11.5px;margin-top:20px;opacity:.8;max-width:300px;}

  header{text-align:center;padding:22px 16px 10px;}
  .castle{font-size:42px;line-height:1;filter:drop-shadow(0 4px 20px rgba(255,206,92,.5));animation:float 4s ease-in-out infinite;display:inline-block;}
  @keyframes float{0%,100%{transform:translateY(0)}50%{transform:translateY(-7px)}}
  header h1{font-family:'Fredoka',sans-serif;font-weight:700;font-size:27px;margin-top:6px;background:linear-gradient(95deg,var(--gold-soft),var(--gold),var(--magenta),var(--cyan));background-size:200% auto;-webkit-background-clip:text;background-clip:text;-webkit-text-fill-color:transparent;animation:shine 6s linear infinite;}
  @keyframes shine{to{background-position:200% center}}
  header p{color:var(--muted);font-size:13px;margin-top:4px;}
  .toolbar{display:flex;justify-content:center;gap:10px;margin-top:12px;}
  .tbtn.ic{width:44px;height:44px;justify-content:center;font-size:19px;padding:0;border-radius:50%;}
  #dedHeart{font-size:18px;}
  .vstamp{position:absolute;bottom:10px;left:0;right:0;text-align:center;font-size:10px;letter-spacing:.5px;color:rgba(255,255,255,.35);font-family:'Nunito',sans-serif;}
  #fabAdd{position:fixed;bottom:22px;right:16px;width:56px;height:56px;border-radius:50%;background:linear-gradient(135deg,var(--magenta),#c44ea0);color:#fff;font-size:30px;font-weight:300;border:none;box-shadow:0 8px 22px rgba(255,111,181,.45);z-index:45;display:none;cursor:pointer;align-items:center;justify-content:center;line-height:1;}
  body.mem #fabAdd{display:flex;}
  .tbtn{display:inline-flex;align-items:center;gap:5px;background:rgba(255,255,255,.06);border:1px solid var(--line);color:var(--gold-soft);padding:6px 11px;border-radius:999px;font-weight:800;font-size:11.5px;cursor:pointer;}
  .tbtn .av{width:20px;height:20px;border-radius:50%;background:rgba(255,255,255,.12);display:flex;align-items:center;justify-content:center;overflow:hidden;font-size:11px;}
  .tbtn .av img{width:100%;height:100%;object-fit:cover;}

  .tabs{position:sticky;top:0;z-index:20;display:flex;gap:6px;padding:12px 0;margin:0 -16px;padding-left:16px;padding-right:16px;background:linear-gradient(180deg,var(--night2) 70%,transparent);backdrop-filter:blur(8px);overflow-x:auto;}
  body.warm .tabs{background:linear-gradient(180deg,var(--warm1) 70%,transparent);}
  .tab{flex:1;min-width:80px;text-align:center;font-family:'Fredoka',sans-serif;font-weight:600;font-size:13px;padding:10px 5px;border-radius:14px;cursor:pointer;background:var(--panel);border:1px solid var(--line);color:var(--muted);transition:transform .2s,background .3s,color .3s,box-shadow .3s;}
  .tab:active{transform:scale(.95);}
  .tab.active{background:linear-gradient(135deg,var(--magenta),#c44ea0);color:#fff;border-color:transparent;box-shadow:0 6px 20px rgba(255,111,181,.4);transform:translateY(-1px);}
  .tab small{display:block;font-size:9.5px;font-weight:600;opacity:.85;margin-top:1px;}

  .tabs .mtab{display:none;}
  body.mem .tabs .gtab{display:none;}
  body.mem .tabs .mtab{display:block;}
  .tab.switch{background:linear-gradient(135deg,rgba(98,230,255,.16),rgba(98,230,255,.06));color:var(--cyan);border-color:rgba(98,230,255,.3);}
  body.mem .tab.switch{background:linear-gradient(135deg,rgba(255,206,92,.16),rgba(255,206,92,.06));color:var(--warmgold);border-color:rgba(255,206,92,.3);}
  .page{display:none;}
  .page.active{display:block;}

  .park-banner{margin:18px 0 6px;padding:18px;border-radius:18px;background:linear-gradient(135deg,var(--panel2),var(--panel));border:1px solid var(--line);position:relative;overflow:hidden;animation:rise .5s ease both;}
  .park-banner::before{content:'';position:absolute;inset:0;background:linear-gradient(120deg,transparent 30%,rgba(255,255,255,.06) 50%,transparent 70%);transform:translateX(-100%);animation:sweep 5s ease-in-out infinite;}
  @keyframes sweep{0%,60%{transform:translateX(-100%)}100%{transform:translateX(100%)}}
  .park-banner h2{font-family:'Fredoka',sans-serif;font-size:21px;font-weight:700;position:relative;}
  .park-banner .sub{color:var(--cyan);font-size:13px;font-weight:700;margin-top:3px;position:relative;}

  .legend{display:flex;gap:8px;flex-wrap:wrap;margin:14px 0 4px;}
  .lg{display:flex;align-items:center;gap:5px;font-size:11.5px;font-weight:700;background:rgba(255,255,255,.05);padding:5px 10px;border-radius:999px;color:var(--muted);}
  .dot{width:9px;height:9px;border-radius:50%;}
  .d-g{background:var(--green)} .d-y{background:var(--yellow)} .d-r{background:var(--red)}

  .tl{margin-top:14px;}
  .item{margin-bottom:11px;}
  .card{background:linear-gradient(150deg,rgba(44,33,97,.92),rgba(36,26,82,.92));border:1px solid var(--line);border-radius:16px;overflow:hidden;transition:transform .2s,border-color .3s,box-shadow .3s;opacity:0;transform:translateY(14px);animation:rise .5s ease forwards;}
  @keyframes rise{to{opacity:1;transform:none}}
  .card:active{transform:scale(.99);}
  .card.open{border-color:rgba(255,206,92,.35);box-shadow:0 8px 28px rgba(0,0,0,.3);}
  .card.done{opacity:.5;}
  .chead{display:flex;align-items:center;gap:10px;padding:14px;cursor:pointer;}
  .emoji{font-size:23px;flex-shrink:0;transition:transform .3s;}
  .card.open .emoji{transform:scale(1.15) rotate(-6deg);}
  .ctitle{flex:1;min-width:0;}
  .ctitle b{display:block;font-family:'Fredoka',sans-serif;font-weight:600;font-size:15px;line-height:1.25;}
  .ctitle .zone{font-size:11.5px;color:var(--muted);font-weight:600;margin-top:2px;}
  .photodot{flex-shrink:0;font-size:11px;color:var(--cyan);font-weight:800;}
  .badge{flex-shrink:0;width:11px;height:11px;border-radius:50%;}
  .chev{flex-shrink:0;color:var(--muted);font-size:12px;transition:transform .3s;}
  .card.open .chev{transform:rotate(180deg);}
  .cbody{max-height:0;overflow:hidden;transition:max-height .45s cubic-bezier(.3,.7,.3,1);}
  .card.open .cbody{max-height:1600px;}
  .cbody-in{padding:0 14px 14px;border-top:1px solid var(--line);margin-top:-1px;padding-top:13px;}
  .timeline-time{display:inline-flex;align-items:center;gap:6px;font-family:'Fredoka',sans-serif;font-weight:600;font-size:12.5px;color:var(--gold-soft);background:rgba(255,206,92,.12);border:1px solid rgba(255,206,92,.25);padding:4px 11px;border-radius:999px;margin-bottom:10px;}
  .cbody p{font-size:13.5px;color:#e3dcff;margin-bottom:9px;}
  .tag{display:inline-block;font-size:11px;font-weight:800;padding:3px 9px;border-radius:7px;margin:0 6px 8px 0;}
  .tag.must{background:rgba(255,206,92,.16);color:var(--gold-soft);}
  .tag.kid{background:rgba(98,230,255,.14);color:var(--cyan);}
  .tag.show{background:rgba(255,111,181,.16);color:var(--magenta);}
  .howto{background:rgba(95,224,137,.08);border-left:3px solid var(--green);padding:10px 12px;border-radius:8px;font-size:12.5px;color:#cdebd6;}
  .howto b{color:var(--green);}
  .howto ol{margin:6px 0 0 16px;padding:0;}
  .howto li{margin-bottom:4px;}
  .maplink{display:inline-flex;align-items:center;gap:7px;margin-top:11px;background:linear-gradient(135deg,rgba(98,230,255,.16),rgba(98,230,255,.08));border:1px solid rgba(98,230,255,.35);color:var(--cyan);text-decoration:none;font-weight:800;font-size:12.5px;padding:9px 14px;border-radius:11px;transition:transform .15s;}
  .maplink:active{transform:scale(.96);}

  .photobox{margin-top:13px;padding-top:12px;border-top:1px dashed var(--line);}
  .photobox .pl{font-size:12px;font-weight:800;color:var(--magenta);margin-bottom:9px;display:flex;align-items:center;gap:6px;}
  .thumbs{display:flex;flex-wrap:wrap;gap:8px;}
  .thumb{position:relative;width:74px;height:74px;border-radius:11px;overflow:hidden;border:1px solid var(--line);animation:pop .3s ease;}
  .thumb img{width:100%;height:100%;object-fit:cover;cursor:pointer;}
  .thumb .who-badge{position:absolute;bottom:0;left:0;right:0;background:rgba(0,0,0,.55);color:#fff;font-size:8.5px;font-weight:800;padding:2px 3px;text-align:center;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;cursor:pointer;}
  .addphoto{width:74px;height:74px;border-radius:11px;border:2px dashed rgba(255,111,181,.4);background:rgba(255,111,181,.08);color:var(--magenta);display:flex;flex-direction:column;align-items:center;justify-content:center;gap:2px;cursor:pointer;font-size:11px;font-weight:800;}
  .addphoto span{font-size:20px;}
  .thumb .cap-dot{position:absolute;top:3px;right:3px;font-size:11px;background:rgba(0,0,0,.55);border-radius:6px;padding:1px 3px;}
  .addphoto.block{width:auto;height:auto;flex-direction:row;gap:6px;padding:9px 13px;border-radius:11px;font-size:12.5px;margin-top:4px;}
  .photorows{display:flex;flex-wrap:wrap;gap:10px;margin-top:10px;}
  .photorow{display:flex;gap:10px;align-items:flex-start;}
  .photorow:not(.nocap){flex-basis:100%;}
  .photorow .thumb{flex:0 0 auto;width:78px;height:78px;}
  .photorow .prcap{flex:1;min-width:0;white-space:pre-wrap;font-size:12.5px;color:#ffeede;background:rgba(0,0,0,.16);border-radius:8px;padding:8px 10px;}
  .photorow .prempty{color:var(--muted);font-style:italic;}
  .photorow.nocap{flex:0 0 auto;}
  .thumb .cap-dot{position:absolute;top:3px;right:3px;font-size:11px;background:rgba(0,0,0,.5);border-radius:6px;padding:1px 3px;}
  .photocap{white-space:pre-wrap;font-size:12.5px;color:#ffeede;background:rgba(0,0,0,.18);border-left:3px solid var(--rose);border-radius:8px;padding:8px 10px;margin-top:8px;}
  .addphoto input{display:none;}

  .special{border:1px dashed rgba(255,206,92,.45);background:rgba(255,206,92,.07);}
  .special .ctitle b{color:var(--gold-soft);}
  .finale{border:1px solid rgba(255,111,181,.5);background:linear-gradient(135deg,rgba(255,111,181,.16),rgba(98,230,255,.09));animation:rise .5s ease forwards, finaleglow 3.5s ease-in-out infinite 1s;}
  @keyframes finaleglow{0%,100%{box-shadow:0 0 14px rgba(255,111,181,.1)}50%{box-shadow:0 0 26px rgba(255,111,181,.3)}}
  .finale .ctitle b{color:#fff;}

  .check{flex-shrink:0;width:23px;height:23px;border-radius:8px;border:2px solid var(--muted);display:flex;align-items:center;justify-content:center;font-size:13px;color:transparent;cursor:pointer;transition:all .25s;}
  .check:active{transform:scale(.8);}
  .card.done .check{background:var(--green);border-color:var(--green);color:#102;animation:pop .3s ease;}
  @keyframes pop{0%{transform:scale(.5)}60%{transform:scale(1.2)}100%{transform:scale(1)}}

  .info-card{background:linear-gradient(150deg,rgba(44,33,97,.92),rgba(36,26,82,.92));border:1px solid var(--line);border-radius:16px;padding:16px;margin-bottom:13px;opacity:0;transform:translateY(14px);animation:rise .5s ease forwards;}
  .info-card h3{font-family:'Fredoka',sans-serif;font-size:16px;font-weight:600;display:flex;align-items:center;gap:8px;margin-bottom:11px;}
  .info-card p,.info-card li{font-size:13.5px;color:#e3dcff;margin-bottom:7px;}
  .info-card ul{padding-left:4px;list-style:none;}
  .info-card li{position:relative;padding-left:20px;}
  .info-card li::before{content:'\2726';position:absolute;left:0;color:var(--gold);font-size:12px;top:1px;}
  .step{display:flex;gap:11px;align-items:flex-start;margin-bottom:12px;}
  .step .n{flex-shrink:0;width:27px;height:27px;border-radius:50%;background:linear-gradient(135deg,var(--magenta),#c44ea0);color:#fff;font-family:'Fredoka',sans-serif;font-weight:700;font-size:13px;display:flex;align-items:center;justify-content:center;box-shadow:0 3px 10px rgba(255,111,181,.3);}
  .step div{font-size:13.5px;color:#e3dcff;}
  .step b{color:var(--cyan);}
  .pill{display:inline-block;background:rgba(98,230,255,.16);color:var(--cyan);font-weight:800;font-size:12px;padding:2px 9px;border-radius:7px;}
  .warn{background:rgba(255,210,74,.1);border:1px solid rgba(255,210,74,.3);border-radius:12px;padding:12px 14px;font-size:13px;color:var(--gold-soft);margin-top:6px;}
  .placerow{display:flex;align-items:center;gap:11px;padding:12px 0;border-bottom:1px solid var(--line);}
  .placerow:last-child{border-bottom:none;}
  .placerow .pe{font-size:21px;}
  .placerow .pi{flex:1;}
  .placerow .pi b{display:block;font-size:13.5px;font-family:'Fredoka',sans-serif;font-weight:500;}
  .placerow .pi span{font-size:11.5px;color:var(--muted);}
  .placerow a{flex-shrink:0;background:linear-gradient(135deg,rgba(98,230,255,.16),rgba(98,230,255,.08));border:1px solid rgba(98,230,255,.35);color:var(--cyan);text-decoration:none;font-weight:800;font-size:11.5px;padding:8px 13px;border-radius:10px;}

  .ded{position:relative;overflow:hidden;border-radius:20px;padding:22px 20px;margin:18px 0 16px;background:linear-gradient(150deg,rgba(255,158,196,.14),rgba(255,206,92,.1));border:1px solid rgba(255,206,92,.25);box-shadow:0 8px 30px rgba(0,0,0,.25);animation:rise .6s ease both;}
  .ded .dhead{display:flex;align-items:center;justify-content:center;gap:10px;cursor:pointer;}
  .ded h2{font-family:'Fredoka',sans-serif;font-size:22px;font-weight:700;color:var(--warmgold);text-align:center;}
  .ded .dhead .chev{color:var(--warmgold);font-size:13px;transition:transform .3s;}
  .ded.collapsed .dhead .chev{transform:rotate(-90deg);}
  .ded .dbody{max-height:600px;overflow:hidden;transition:max-height .4s ease;}
  .ded.collapsed .dbody{max-height:0;}
  .ded .dtext{font-size:13.5px;color:#ffeede;margin-top:12px;line-height:1.65;text-align:center;font-style:italic;}
  .ded .dsign{display:block;margin-top:14px;text-align:center;font-family:'Fredoka',sans-serif;font-weight:600;color:var(--rose);font-size:14px;font-style:normal;}
  .ded .dcount{display:flex;justify-content:center;gap:18px;margin-top:16px;}
  .ded .dcount div{text-align:center;}
  .ded .dcount b{display:block;font-family:'Fredoka',sans-serif;font-size:20px;color:var(--warmgold);}
  .ded .dcount span{font-size:10.5px;color:#ffd9c0;font-weight:700;}

  .collapse-head{display:flex;align-items:center;gap:9px;cursor:pointer;}
  .collapse-head .chev{margin-left:auto;}
  .mform{background:linear-gradient(150deg,rgba(58,35,48,.92),rgba(42,24,48,.92));border:1px solid rgba(255,206,92,.18);border-radius:16px;padding:16px;margin-bottom:14px;}
  .mform>.collapse-head h3{font-family:'Fredoka',sans-serif;font-size:16px;color:var(--warmgold);}
  .mform-body{max-height:0;overflow:hidden;transition:max-height .4s ease;}
  .mform.open .mform-body{max-height:1200px;margin-top:13px;}
  .mform.open .collapse-head .chev{transform:rotate(180deg);}
  .mform input,.mform textarea{width:100%;background:rgba(0,0,0,.25);border:1px solid var(--line);border-radius:11px;padding:11px 13px;color:var(--text);font-family:'Nunito',sans-serif;font-size:14px;margin-bottom:10px;resize:vertical;}
  .mform input::placeholder,.mform textarea::placeholder{color:var(--muted);}
  .placewrap{display:flex;gap:8px;}
  .placewrap input{flex:1;}
  .choosebtn{flex-shrink:0;background:rgba(255,206,92,.14);border:1px solid rgba(255,206,92,.3);color:var(--warmgold);border-radius:11px;padding:0 14px;font-weight:800;font-size:12.5px;cursor:pointer;margin-bottom:10px;}
  .formphotos{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:10px;}
  .btn{background:linear-gradient(135deg,var(--magenta),#c44ea0);color:#fff;border:none;font-family:'Fredoka',sans-serif;font-weight:600;font-size:14px;padding:12px;border-radius:12px;width:100%;cursor:pointer;box-shadow:0 6px 18px rgba(255,111,181,.35);transition:transform .15s;}
  .btn:active{transform:scale(.97);}
  .btn.sec{background:transparent;border:1px solid rgba(255,206,92,.4);color:var(--warmgold);box-shadow:none;}
  .btn.tiny{font-size:12px;padding:9px;}
  .addfotobtn .plus{display:inline-flex;align-items:center;justify-content:center;width:18px;height:18px;border-radius:50%;background:var(--magenta);color:#fff;font-weight:900;font-size:14px;line-height:1;}
  .expandbar{display:flex;gap:10px;margin-bottom:10px;}
  .expandbar .btn{flex:1;}
  .btnrow{display:flex;gap:10px;width:100%;}
  .btnrow .btn{flex:1;padding:12px 10px;font-size:13.5px;}
  .lbtns{max-width:520px;}
  .timeline{position:relative;padding-left:62px;margin-top:6px;}
  .timeline::before{content:'';position:absolute;left:54px;top:8px;bottom:8px;width:2px;background:linear-gradient(180deg,var(--rose),var(--warmgold));opacity:.55;}
  .tlitem{position:relative;margin-bottom:16px;}
  .tldot{position:absolute;left:-14px;top:7px;width:12px;height:12px;border-radius:50%;background:var(--warmgold);box-shadow:0 0 10px rgba(255,206,92,.6);border:2px solid var(--warm1);}
  .tldatedot{position:absolute;left:-62px;top:3px;width:46px;text-align:right;font-family:'Fredoka',sans-serif;font-weight:700;font-size:10.5px;color:var(--gold);line-height:1.15;}
  .tlcard{background:linear-gradient(150deg,rgba(58,35,48,.92),rgba(42,24,48,.92));border:1px solid rgba(255,206,92,.16);border-radius:14px;padding:13px;animation:rise .4s ease;}
  .tldate{font-family:'Fredoka',sans-serif;font-weight:700;font-size:12px;color:var(--gold);}
  .tltitle{font-family:'Fredoka',sans-serif;font-weight:600;font-size:15px;color:#fff;margin-top:2px;display:flex;align-items:center;gap:8px;flex-wrap:wrap;}
  .tltitle .tlauthor{font-size:11.5px;font-weight:700;color:#ffd9c0;}
  .tlcard{padding:12px;}
  .tlcard .mplace{font-size:10.5px;padding:2px 9px;}
  .tlcard .tlplaces{gap:6px;margin-top:7px;}
  .tlcard .photocap{margin-top:9px;font-size:12.5px;}
  .tlcard .photorows{margin-top:10px;gap:9px;}
  .tlcard .photorow .thumb{width:64px;height:64px;}
  .ineditor .ie-input{width:100%;background:rgba(0,0,0,.25);border:1px solid var(--line);border-radius:11px;padding:10px 12px;color:var(--text);font-family:'Nunito',sans-serif;font-size:14px;margin-bottom:8px;resize:vertical;}
  .ineditor .placewrap{margin-bottom:6px;}
  .tlcard .mmeta{font-size:11.5px;color:#ffd9c0;display:flex;gap:10px;flex-wrap:wrap;margin-top:4px;}
  .tlcard .thumbs{margin-top:9px;}
  .tlcard .photocap{margin-top:8px;}
  .syncbtn{width:100%;background:linear-gradient(135deg,rgba(255,158,196,.16),rgba(255,206,92,.12));border:1px solid rgba(255,206,92,.3);color:var(--warmgold);font-family:'Fredoka',sans-serif;font-weight:600;font-size:14px;padding:13px;border-radius:14px;cursor:pointer;margin:6px 0 14px;display:flex;align-items:center;justify-content:center;gap:8px;}
  .empty{text-align:center;color:#ffd9c0;font-size:13px;padding:24px 10px;opacity:.75;}
  .moment{background:linear-gradient(150deg,rgba(58,35,48,.92),rgba(42,24,48,.92));border:1px solid rgba(255,206,92,.16);border-radius:16px;padding:15px;margin-bottom:12px;animation:rise .4s ease;}
  .moment .mhead{display:block;cursor:pointer;}
  .moment .mhtop{display:flex;align-items:center;gap:9px;}
  .moment .mhmeta{display:flex;flex-wrap:wrap;gap:7px;margin-top:8px;}
  .moment .mplace{font-weight:800;font-size:11.5px;padding:3px 10px;border-radius:999px;border:1px solid;}
  .moment .mtag{font-size:11px;font-weight:700;color:#ffd9c0;background:rgba(255,255,255,.06);padding:3px 9px;border-radius:999px;}
  .pc-disney{color:#ff6fb5;background:rgba(255,111,181,.14);border-color:rgba(255,111,181,.4);}
  .pc-paris{color:#7db4ff;background:rgba(90,140,255,.14);border-color:rgba(90,140,255,.4);}
  .pc-bx{color:#ffce5c;background:rgba(255,206,92,.14);border-color:rgba(255,206,92,.4);}
  .pc-bg{color:#5fe089;background:rgba(95,224,137,.14);border-color:rgba(95,224,137,.4);}
  .pc-ams{color:#ff9a62;background:rgba(255,154,98,.14);border-color:rgba(255,154,98,.4);}
  .pc-def{color:var(--warmgold);background:rgba(255,206,92,.12);border-color:rgba(255,206,92,.35);}
  .moment .mtitle{font-family:'Fredoka',sans-serif;font-weight:600;font-size:16px;flex:1;color:#fff;}
  .moment .mdel{background:none;border:none;color:var(--red);font-size:17px;cursor:pointer;opacity:.8;}
  .moment .medit{color:var(--cyan);}
  .moment .chev{color:#ffd9c0;font-size:12px;transition:transform .3s;}
  .moment .mbody{max-height:0;overflow:hidden;transition:max-height .4s ease;}
  .moment.open .mbody{max-height:1600px;margin-top:9px;}
  .moment.open .mhead .chev{transform:rotate(180deg);}
  .moment .mmeta{font-size:11.5px;color:#ffd9c0;display:flex;flex-wrap:wrap;gap:10px;}
  .moment .mnote{font-size:13.5px;color:#ffeede;margin-top:9px;line-height:1.55;}

  .modal{position:fixed;inset:0;z-index:50;background:rgba(10,7,24,.85);backdrop-filter:blur(6px);display:none;align-items:center;justify-content:center;padding:20px;}
  .modal.open{display:flex;animation:fadein .25s ease;}
  @keyframes fadein{from{opacity:0}to{opacity:1}}
  .modal-box{background:var(--panel);border:1px solid var(--line);border-radius:18px;padding:18px;max-width:520px;width:100%;max-height:85vh;overflow:auto;}
  .modal-box h3{font-family:'Fredoka',sans-serif;font-size:17px;margin-bottom:6px;}
  .modal-box p{font-size:12.5px;color:var(--muted);margin-bottom:12px;}
  .modal-box textarea{width:100%;height:130px;background:rgba(0,0,0,.3);border:1px solid var(--line);border-radius:11px;padding:11px;color:var(--text);font-family:monospace;font-size:11px;margin-bottom:12px;}
  .syncopts{display:flex;flex-direction:column;gap:10px;margin-bottom:6px;}
  .modal-box .small{font-size:11px;color:var(--muted);margin:-2px 0 10px;}
  .placelist{display:flex;flex-wrap:wrap;gap:8px;max-height:50vh;overflow:auto;margin-bottom:12px;}
  .placelist button{background:rgba(255,255,255,.06);border:1px solid var(--line);color:var(--text);border-radius:10px;padding:9px 12px;font-size:12.5px;font-weight:700;cursor:pointer;}
  .placelist button.picked{background:rgba(95,224,137,.18);border-color:rgba(95,224,137,.5);color:#bff0cf;}
  .plgroup{width:100%;font-size:11px;font-weight:800;color:var(--gold-soft);margin-top:6px;}

  .lightbox{position:fixed;inset:0;z-index:60;background:rgba(0,0,0,.92);display:none;align-items:center;justify-content:center;flex-direction:column;padding:20px;gap:14px;}
  .lightbox.open{display:flex;animation:fadein .25s ease;}
  .lightbox img{max-width:100%;max-height:52vh;border-radius:14px;}
  .lbnav{position:fixed;top:50%;transform:translateY(-50%);background:rgba(255,255,255,.12);border:none;color:#fff;font-size:30px;width:46px;height:46px;border-radius:50%;cursor:pointer;z-index:62;display:flex;align-items:center;justify-content:center;}
  .lbnav.prev{left:10px;} .lbnav.next{right:10px;}
  .lbpos{color:#bbb;font-size:12px;font-weight:800;}
  .lightbox #lbCaption{width:100%;max-width:520px;min-height:74px;background:rgba(255,255,255,.08);border:1px solid var(--line);border-radius:12px;padding:11px;color:#fff;font-family:'Nunito',sans-serif;font-size:14px;resize:vertical;}
  .lightbox .lbinfo{color:#ddd;font-size:12.5px;text-align:center;}
  .lightbox .lbcompliment{color:var(--gold-soft);font-family:'Fredoka',sans-serif;font-weight:600;font-size:16px;text-align:center;max-width:520px;}
  #toast{position:fixed;left:50%;bottom:26px;transform:translateX(-50%) translateY(20px);background:rgba(20,14,40,.96);border:1px solid var(--line);color:var(--gold-soft);padding:11px 18px;border-radius:999px;font-weight:800;font-size:13px;z-index:100;opacity:0;transition:all .3s;pointer-events:none;box-shadow:0 8px 24px rgba(0,0,0,.45);}
  #toast.show{opacity:1;transform:translateX(-50%) translateY(0);}
  .moment .mphotos{font-size:11px;color:var(--cyan);font-weight:800;}
  .lightbox .lbtns{display:flex;gap:12px;}

  #albumDateFloat{position:fixed;right:10px;top:118px;z-index:30;display:none;background:rgba(20,14,40,.92);border:1px solid rgba(255,206,92,.35);color:var(--warmgold);font-family:'Fredoka',sans-serif;font-weight:700;font-size:11.5px;padding:5px 11px;border-radius:999px;box-shadow:0 4px 14px rgba(0,0,0,.4);}
  .authchip{display:inline-flex;align-items:center;gap:5px;}
  .achip-av{width:18px;height:18px;border-radius:50%;overflow:hidden;display:inline-flex;align-items:center;justify-content:center;background:rgba(255,255,255,.12);font-size:10px;}
  .achip-av img{width:100%;height:100%;object-fit:cover;}
  a.mplace{text-decoration:none;}
  .albumfilters{display:flex;gap:8px;margin-bottom:8px;flex-wrap:wrap;align-items:center;}
  #albumSearch{flex:1;min-width:140px;background:rgba(0,0,0,.25);border:1px solid var(--line);border-radius:12px;padding:11px 13px;color:var(--text);font-family:'Nunito',sans-serif;font-size:14px;}
  .albumfilters .btn.tiny{flex:0 0 auto;width:auto;padding:9px 12px;}
  .memtop{margin:14px 0 10px;background:linear-gradient(150deg,rgba(255,158,196,.12),rgba(255,206,92,.08));border:1px solid rgba(255,206,92,.2);border-radius:14px;padding:10px 14px;}
  .memtop-count{display:flex;justify-content:center;gap:20px;}
  .memtop-count div{text-align:center;}
  .memtop-count b{display:block;font-family:'Fredoka',sans-serif;font-size:17px;color:var(--warmgold);line-height:1.05;}
  .memtop-count span{font-size:8.5px;color:#ffd9c0;font-weight:800;text-transform:uppercase;letter-spacing:.4px;}
  .filterbar{display:flex;gap:7px;align-items:stretch;margin-bottom:10px;}
  .fbtn{height:40px;border:1px solid var(--line);background:rgba(255,255,255,.06);color:var(--gold-soft);font-family:'Nunito',sans-serif;font-weight:800;font-size:12.5px;border-radius:11px;padding:0 12px;cursor:pointer;display:inline-flex;align-items:center;justify-content:center;white-space:nowrap;flex:0 0 auto;}
  .fbtn.fgrow{flex:1;min-width:0;overflow:hidden;text-overflow:ellipsis;}
  .filterbar.even .fbtn{flex:1;min-width:0;}
  input.fbtn{font-weight:600;color:var(--text);background:rgba(0,0,0,.25);text-align:left;}
  input.fbtn::placeholder{color:var(--muted);}
  body.mem .fbtn{color:var(--warmgold);}
  body.mem input.fbtn{color:var(--text);}
  .daychips.picker{flex-wrap:nowrap;overflow-x:auto;scrollbar-width:none;-ms-overflow-style:none;padding-bottom:4px;}
  .daychips.picker::-webkit-scrollbar{display:none;}
  .albumfilters-top{display:flex;gap:8px;align-items:flex-end;margin-bottom:8px;}
  .ff{display:flex;flex-direction:column;gap:3px;min-width:0;}
  .ff-grow{flex:1;}
  .fflabel{font-size:9.5px;color:#ffd9c0;font-weight:800;text-transform:uppercase;letter-spacing:.4px;padding-left:3px;}
  .ff input{width:100%;background:rgba(0,0,0,.25);border:1px solid var(--line);border-radius:10px;padding:8px 10px;color:var(--text);font-family:'Nunito',sans-serif;font-size:13px;}
  .ff input[type=date]{width:138px;min-width:138px;}
  .fflabel2{font-size:11.5px;color:#ffd9c0;font-weight:800;margin:4px 0 6px;}
  .chipsel{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:10px;}
  .chipsel .selchip{background:rgba(255,206,92,.14);border:1px solid rgba(255,206,92,.35);color:var(--warmgold);font-weight:700;font-size:12px;padding:5px 10px;border-radius:999px;display:inline-flex;align-items:center;gap:7px;}
  .chipsel .selchip b{cursor:pointer;color:var(--red);font-size:13px;}
  .daychips{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:10px;}
  .daychip{width:38px;height:38px;border-radius:10px;border:1px solid var(--line);background:rgba(255,255,255,.06);color:var(--muted);font-weight:800;font-size:13px;cursor:pointer;display:flex;align-items:center;justify-content:center;}
  .daychip.on{background:linear-gradient(135deg,var(--magenta),#c44ea0);color:#fff;border-color:transparent;}
  .daychips.small .daychip{width:33px;height:33px;font-size:12px;border-radius:9px;}
  .diaryfilter{margin-bottom:10px;}
  .albumchips{display:flex;gap:7px;overflow-x:auto;padding:2px;margin-bottom:8px;-webkit-overflow-scrolling:touch;scrollbar-width:none;-ms-overflow-style:none;}
  .albumchips::-webkit-scrollbar{display:none;height:0;}
  .achip{flex:0 0 auto;background:rgba(255,255,255,.06);border:1px solid var(--line);color:var(--muted);font-weight:800;font-size:12px;padding:7px 12px;border-radius:999px;cursor:pointer;white-space:nowrap;transition:all .2s;}
  .achip.active{background:linear-gradient(135deg,var(--magenta),#c44ea0);color:#fff;border-color:transparent;box-shadow:0 4px 12px rgba(255,111,181,.3);}
  .albumfilters-row{display:flex;gap:8px;align-items:center;}
  .albumfilters-row .btn.tiny{flex:0 0 auto;width:auto;padding:9px 12px;}
  .modal-x{position:absolute;top:8px;right:12px;background:none;border:none;color:#fff;font-size:20px;cursor:pointer;opacity:.8;}
  .ded-modal{position:relative;text-align:center;background:linear-gradient(150deg,rgba(58,35,48,.98),rgba(42,24,48,.98));border:1px solid rgba(255,206,92,.3);}
  .ded-modal .ded-h{font-family:'Fredoka',sans-serif;color:var(--warmgold);font-size:23px;}
  .ded-modal .dtext{font-size:14px;color:#ffeede;margin-top:12px;line-height:1.7;font-style:italic;}
  .ded-modal .dsign{display:block;margin-top:14px;font-family:'Fredoka',sans-serif;font-weight:600;color:var(--rose);font-size:15px;}
  .footnote{text-align:center;color:var(--muted);font-size:11px;margin:20px 0 6px;opacity:.7;}
</style>
</head>
<body>
<div class="stars"></div>
<div class="stars2"></div>
<button id="fabAdd" title="Adicionar momento">＋</button>

<!-- SPLASH -->
<div class="splash" id="splash">
  <button class="splash-corner left" id="splashGear" title="Configurações">⚙️</button>
  <button class="splash-corner right" id="splashGuide" title="Guia da Disney">🗺️ Guia</button>
  <div class="scastle">🏰</div>
  <h1>Preparados para a Eurotrip?</h1>
  <div class="sub">Paris, Disney, Bruxelas, Bruges e Amsterdam. Vamos viver tudo isso juntos.</div>
  <div class="who-q">Quem é você?</div>
  <div class="avatars" id="avatars"></div>
  <input id="guestName" placeholder="Seu nome" maxlength="20" style="display:none">
  <div class="paths" id="paths">
    <button class="pbtn mem" data-go="mem">📷 Nossas memórias</button>
  </div>
  <div class="tip">Toque na sua foto para escolher quem é você. Para mudar a foto de perfil, toque no 📷 do seu avatar.</div>
  <div class="vstamp" id="vstamp">versão 13 · 8 jun</div>
</div>
<script>
/* Tela inicial independente: garante que os avatares sempre apareçam */
(function(){
  var PEOPLE=["Edson","Maria","Thaysa"];
  function prof(n){try{return localStorage.getItem('profile_'+n)||'';}catch(e){return '';}}
  function esc(x){return (''+x).replace(/&/g,'&amp;').replace(/"/g,'&quot;');}
  function render(){
    var c=document.getElementById('avatars');if(!c)return;
    var sel=window.__splashSel||null,h='';
    PEOPLE.forEach(function(n){var p=prof(n);h+='<div class="avatar'+(sel===n?' sel':'')+'" data-name="'+esc(n)+'"><div class="aimg">'+(p?'<img src="'+esc(p)+'">':n.charAt(0))+'</div><label class="acam">📷<input type="file" accept="image/*" data-prof="'+esc(n)+'"></label><span>'+esc(n)+'</span></div>';});
    h+='<div class="avatar'+(sel==='__guest'?' sel':'')+'" data-name="__guest"><div class="aimg">👤</div><span>Convidado</span></div>';
    c.innerHTML=h;
  }
  window.__renderAvatars=render;
  var c=document.getElementById('avatars');
  if(c){
    c.addEventListener('click',function(e){var a=e.target.closest('.avatar');if(!a||e.target.closest('.acam'))return;window.__splashSel=a.getAttribute('data-name');var g=document.getElementById('guestName');if(g)g.style.display=(window.__splashSel==='__guest')?'block':'none';var p=document.getElementById('paths');if(p)p.classList.add('show');render();});
    c.addEventListener('change',function(e){var inp=e.target.closest('[data-prof]');if(!inp||!e.target.files||!e.target.files[0])return;var r=new FileReader();r.onload=function(){try{localStorage.setItem('profile_'+inp.getAttribute('data-prof'),r.result);}catch(_){}render();try{if(window.refreshWhoChip)window.refreshWhoChip();}catch(_){}};r.readAsDataURL(e.target.files[0]);});
  }
  document.querySelectorAll('.pbtn').forEach(function(b){b.addEventListener('click',function(){
    var nm=window.__splashSel||'Convidado';
    if(nm==='__guest'){var g=document.getElementById('guestName');nm=(g&&g.value||'').trim()||'Convidado';}
    try{localStorage.setItem('username',nm);}catch(_){}
    var go=b.getAttribute('data-go')||'mem';
    var sp=document.getElementById('splash');if(sp)sp.classList.add('hide'); /* SEMPRE entra, sem alerta */
    try{
      if(window.__enterApp){window.__enterApp(go);return;}
      try{if(window.refreshWhoChip)window.refreshWhoChip();}catch(_){}
      try{if(window.reRenderAll)window.reRenderAll();}catch(_){}
      document.body.classList.add('mem');document.body.classList.add('warm');
      document.querySelectorAll('.page').forEach(function(p){p.classList.toggle('active',p.id===go);});
      document.querySelectorAll('.tab').forEach(function(t){t.classList.toggle('active',t.getAttribute('data-tab')===go);});
      try{if(window.activateTab)window.activateTab(go);}catch(_){}
    }catch(_){}
  });});
  render();
})();
</script>

<div class="wrap">
  <header>
    <div class="castle">🏰</div>
    <h1 id="hTitle">Nosso Guia Disney</h1>
    <p id="hSub">Edson · Maria · Thaysa <span style="opacity:.8">🐾 Lilo no coração</span></p>
    <div class="toolbar">
      <div class="tbtn ic" id="homeBtn" title="Início">🏠</div>
      <div class="tbtn ic" id="syncTopBtn" title="Sincronizar">🔄</div>
      <div class="tbtn ic" id="dedHeart" title="Dedicatória">💛</div>
      <div class="tbtn" id="toggleBtn" title="Trocar de seção">📷 Memórias</div>
    </div>
  </header>

  <div class="tabs">
    <div class="tab gtab active" data-tab="d1">Dia 1<small>Adventure</small></div>
    <div class="tab gtab" data-tab="d2">Dia 2<small>Disneyland</small></div>
    <div class="tab gtab" data-tab="info">Info<small>Como ir</small></div>
    <div class="tab mtab" data-tab="mem">Diário<small>Momentos</small></div>
    <div class="tab mtab" data-tab="album">Álbum<small>Linha do tempo</small></div>
  </div>

  <section class="page active" id="d1">
    <div class="park-banner"><h2>🎬 Disney Adventure World</h2><div class="sub">Antigo Walt Disney Studios</div></div>
    <div class="legend"><span class="lg"><span class="dot d-g"></span>Tranquila</span><span class="lg"><span class="dot d-y"></span>Emoção moderada</span><span class="lg"><span class="dot d-r"></span>Radical</span></div>
    <div class="tl" id="tl-d1"></div>
  </section>

  <section class="page" id="d2">
    <div class="park-banner"><h2>🏰 Disneyland Park</h2><div class="sub">O parque clássico do Castelo</div></div>
    <div class="legend"><span class="lg"><span class="dot d-g"></span>Tranquila</span><span class="lg"><span class="dot d-y"></span>Emoção moderada</span><span class="lg"><span class="dot d-r"></span>Radical</span></div>
    <div class="tl" id="tl-d2"></div>
  </section>

  <section class="page" id="mem">
    <div class="memtop">
      <div class="memtop-count">
        <div><b id="cMoments">0</b><span>Momentos</span></div>
        <div><b id="cPhotos">0</b><span>Fotos</span></div>
        <div><b>4–15 jun</b><span>Eurotrip 2026</span></div>
      </div>
    </div>

    <div class="mform" id="mform">
      <div class="collapse-head" id="mformHead"><h3>✨ Adicionar um momento</h3><span class="chev">▼</span></div>
      <div class="mform-body">
        <input id="mTitle" placeholder="Título (opcional)">
        <div class="fflabel2">📍 Locais (pode adicionar vários)</div>
        <div class="placewrap">
          <input id="mPlace" list="placeSuggestions" placeholder="Digite ou escolha...">
          <button class="choosebtn" id="addPlaceBtn">+</button>
          <button class="choosebtn" id="choosePlace">📍 Lista</button>
        </div>
        <datalist id="placeSuggestions"></datalist>
        <div class="chipsel" id="formPlaces"></div>
        <div class="fflabel2">📅 Dias da viagem (obrigatório, de um dia até outro)</div>
        <button class="btn sec tiny daysbtn" id="formDaysBtn" style="width:auto;margin-bottom:12px">📅 Escolher dias</button>
        <textarea id="mNote" rows="2" placeholder="Lembrança ou descrição (opcional)"></textarea>
        <div class="formphotos" id="formPhotos"></div>
        <label class="btn sec tiny addfotobtn" style="display:block;text-align:center;margin-bottom:10px;cursor:pointer"><span class="plus">+</span> Adicionar foto<input type="file" accept="image/*" id="mPhotoInput" multiple style="display:none"></label>
        <button class="btn" id="addMoment">💛 Salvar momento</button>
      </div>
    </div>

    <div class="filterbar even">
      <button id="diaryDaysBtn" class="fbtn">📅 Dias</button>
      <button id="expandAll" class="fbtn">Expandir</button>
      <button id="collapseAll" class="fbtn">Recolher</button>
    </div>
    <div id="momentsList"></div>

  </section>

  <section class="page" id="album">
    <div class="ded">
      <h2>📸 Linha do tempo</h2>
      <div class="dtext">Todos os momentos da nossa Eurotrip, em ordem, de todo mundo. Role e reviva nossa história.</div>
    </div>
    <div class="albumfilters">
      <div class="filterbar">
        <input id="albumSearch" class="fbtn fgrow" placeholder="🔎 Buscar...">
        <button id="albumDaysBtn" class="fbtn">📅 Dias</button>
        <button id="albumClear" class="fbtn">Limpar</button>
      </div>
      <div class="albumchips" id="albumChips">
        <button class="achip active" data-city="">✨ Todos</button>
        <button class="achip" data-city="pc-paris">🗼 Paris</button>
        <button class="achip" data-city="pc-disney">🏰 Disney</button>
        <button class="achip" data-city="pc-bx">🍫 Bruxelas</button>
        <button class="achip" data-city="pc-bg">🛶 Bruges</button>
        <button class="achip" data-city="pc-ams">🌷 Amsterdam</button>
      </div>
    </div>
    <div id="albumFeed"></div>
  </section>

  <section class="page" id="info">
    <div class="info-card">
      <h3>🚇 Como chegar do hotel</h3>
      <div class="step"><span class="n">1</span><div>Saímos do hotel e, como a padaria perto fecha no domingo, compramos algo rápido de comer no caminho.</div></div>
      <div class="step"><span class="n">2</span><div>Na estação <b>Mairie de Montrouge</b>, pegamos o <span class="pill">Metrô 4</span> na direção <b>Porte de Clignancourt</b> e descemos na estação <b>Nation</b>.</div></div>
      <div class="step"><span class="n">3</span><div>Em Nation, pegamos o <span class="pill">RER A</span> na direção <b>Marne la Vallée Chessy</b>. Acabamos pegando o trem errado e nos atrasamos um pouco.</div></div>
      <div class="step"><span class="n">4</span><div>Por causa do trem errado, resolvemos ir direto ao <b>Primark</b>, que abria às 11h, e almoçamos no shopping antes do parque.</div></div>
      <div class="warn">⚠️ Vale lembrar que nem todo RER A vai até <b>Marne la Vallée Chessy</b>, alguns trens param antes. Foi assim que pegamos o errado.<br><br>⚠️ Também pode haver greve afetando as linhas, então vale conferir o app do transporte.</div>
    </div>
    <div class="info-card">
      <h3>📍 Localizações (toque para abrir o mapa)</h3>
      <div class="placerow"><span class="pe">🏨</span><div class="pi"><b>B&B Hotel Porte d'Orléans</b><span>Bd Romain Rolland 53-55, Montrouge</span></div><a href="https://www.google.com/maps/search/?api=1&query=B%26B%20Hotel%20Paris%20Porte%20d%27Orl%C3%A9ans&query_place_id=ChIJ1WY-AMlx5kcRPYolH3-iRlY" target="_blank">Mapa</a></div>
      <div class="placerow"><span class="pe">🚇</span><div class="pi"><b>Estação Mairie de Montrouge</b><span>Metrô Linha 4, direção Porte de Clignancourt</span></div><a href="https://www.google.com/maps/search/?api=1&query=Mairie%20de%20Montrouge&query_place_id=ChIJQVV_yapx5kcR0Q-hLHu4bCk" target="_blank">Mapa</a></div>
      <div class="placerow"><span class="pe">🎬</span><div class="pi"><b>Disney Adventure World</b><span>Chessy, abre às 9h30</span></div><a href="https://www.google.com/maps/search/?api=1&query=Disney%20Adventure%20World%20Chessy&query_place_id=ChIJ_YETR4Ad5kcRyKP2sKsvtSE" target="_blank">Mapa</a></div>
      <div class="placerow"><span class="pe">🏰</span><div class="pi"><b>Disneyland Park</b><span>Bd de Parc, Chessy, abre às 9h30</span></div><a href="https://www.google.com/maps/search/?api=1&query=Disneyland%20Park%20Paris&query_place_id=ChIJf9hphiUd5kcR5RdeomHtvFA" target="_blank">Mapa</a></div>
      <div class="placerow"><span class="pe">🛍️</span><div class="pi"><b>Primark Val d'Europe</b><span>CC Val d'Europe, Serris, abre 11h no domingo</span></div><a href="https://www.google.com/maps/search/?api=1&query=Primark%20Val%20d%27Europe&query_place_id=ChIJPXYiDbkd5kcRUNIX6Bq2tlc" target="_blank">Mapa</a></div>
    </div>
    <div class="info-card">
      <h3>🛍️ Primark (Dia 1, ao meio-dia)</h3>
      <p>Fica no shopping <b>Val d'Europe</b>, a uma estação de RER A da Disney. É bem grande e tem a Primark dentro.</p>
      <ul><li>Saímos do parque por volta das 11h e pegamos o RER A por uma parada até Val d'Europe.</li><li>Guardem o comprovante de entrada do dia, porque ele vale para voltar ao parque.</li><li>Almocem por lá, que costuma sair mais em conta, e voltem por volta das 13h com as filas mais calmas.</li><li>No domingo a Primark abre às 11h.</li></ul>
    </div>
    <div class="info-card">
      <h3>🎯 Estratégia de filas</h3>
      <ul><li>Cheguem na abertura e corram direto para a primeira atração da lista. É aí que vocês ganham tempo nas filas.</li><li>A primeira atração de cada dia (Crush's Coaster e Hyperspace Mountain) é a que mais lota, por isso vem logo no começo.</li><li>Procurem a placa "Single Rider" em algumas atrações como Crush's e RC Racer. Ela adianta a fila se vocês aceitarem sentar separados.</li><li>As filas costumam diminuir durante as paradas e shows e também perto do fechamento.</li></ul>
    </div>
    <div class="info-card">
      <h3>📱 App Disneyland Paris</h3>
      <p>Vale baixar antes de ir. No app vocês têm:</p>
      <ul><li>Mapa interativo de cada parque.</li><li>Tempo de fila em tempo real. Se uma atração estiver muito cheia, pulem e voltem depois.</li><li>Horários dos shows e das paradas do dia, que mudam conforme a data, então sempre confiram ao chegar.</li><li>Cardápios e opções de onde comer.</li></ul>
    </div>
    <div class="info-card">
      <h3>🍔 Comida e dicas finais</h3>
      <ul><li>Levem os lanches do Carrefour na mochila, porque a comida dentro do parque é cara.</li><li>Levem uma garrafa de água, já que há bebedouros pelo parque.</li><li>Usem calçado confortável, porque caminhamos bastante durante o dia inteiro.</li><li>Levem protetor solar e um casaco fininho para a noite, na hora dos shows de encerramento.</li><li>Levem um carregador portátil, porque o app consome bastante bateria.</li></ul>
    </div>
    <div class="footnote">A Adventure World reabriu recentemente, então confiram os caminhos no mapa físico ao entrar. Bom passeio!</div>
  </section>
</div>

<!-- GEAR / SETTINGS -->
<div class="modal" id="gearModal">
  <div class="modal-box">
    <h3>⚙️ Configurações</h3>
    <div class="syncopts">
      <button class="btn" id="gFullHtml">💾 Copiar site completo (para o GitHub)</button>
    </div>
    <div class="small">O "site completo" gera o index.html já com tudo embutido, pronto para colar no GitHub e salvar para sempre.</div>
    <button class="btn sec" id="gearClose" style="margin-top:6px">Fechar</button>
  </div>
</div>

<!-- SYNC MODAL -->
<div class="modal" id="syncModal">
  <div class="modal-box">
    <h3>🔄 Sincronizar com a família</h3>
    <p>Exporte um arquivo com suas fotos e momentos e envie para outro celular. Lá, use Importar para abrir o arquivo e carregar tudo. Ao importar, tudo é somado, nunca substituído.</p>
    <div class="syncopts">
      <button class="btn" id="optExport">Exportar (baixar arquivo)</button>
      <button class="btn sec" id="optImport">Importar (abrir arquivo)</button>
    </div>
    <input type="file" id="importFile" accept=".txt,.json,application/json,text/plain" style="display:none">
    <button class="btn sec" id="syncClose" style="margin-top:8px">Fechar</button>
  </div>
</div>

<!-- TEXT MODAL -->
<div class="modal" id="modal">
  <div class="modal-box">
    <h3 id="modalTitle">Código</h3>
    <p id="modalDesc"></p>
    <textarea id="modalText"></textarea>
    <div class="btnrow"><button class="btn" id="modalAction">Copiar</button><button class="btn sec" id="modalClose">Fechar</button></div>
  </div>
</div>

<!-- PLACE PICKER MODAL -->
<div class="modal" id="placeModal">
  <div class="modal-box">
    <h3>📍 Onde foi?</h3>
    <p>Toque para escolher, ou feche e digite à mão.</p>
    <div class="placelist" id="placeList"></div>
    <button class="btn sec" id="placeClose">Fechar</button>
  </div>
</div>

<div id="albumDateFloat"></div>

<!-- DEDICATION POPUP -->
<div class="modal" id="dedModal">
  <div class="modal-box ded-modal">
    <button class="modal-x" id="dedClose">✕</button>
    <h2 class="ded-h">💛 Nossas Memórias</h2>
    <div class="dtext" id="dedText"></div>
    <span class="dsign">Com amor, da nossa família 🐾</span>
  </div>
</div>

<!-- FORM PHOTO CAPTION -->
<div class="modal" id="capModal">
  <div class="modal-box">
    <h3>📝 Descrição da foto</h3>
    <img id="capImg" style="width:100%;max-height:38vh;object-fit:contain;border-radius:12px;margin-bottom:10px;">
    <textarea id="capText" placeholder="Escreva a descrição desta foto... pode usar parágrafos." style="width:100%;min-height:80px;background:rgba(0,0,0,.25);border:1px solid var(--line);border-radius:11px;padding:11px;color:var(--text);font-family:'Nunito',sans-serif;font-size:14px;resize:vertical;margin-bottom:12px;"></textarea>
    <div class="btnrow"><button class="btn" id="capSave">Salvar</button><button class="btn sec" id="capClose">Fechar</button></div>
  </div>
</div>

<!-- DAY RANGE PICKER -->
<div class="modal" id="dayModal">
  <div class="modal-box">
    <h3>📅 Escolha os dias</h3>
    <p>Toque no primeiro dia e depois no último. Ele seleciona o intervalo (de um dia até outro).</p>
    <div class="daychips picker" id="dayPicker"></div>
    <div class="btnrow"><button class="btn" id="dayApply">Aplicar</button><button class="btn sec" id="dayClear">Fechar</button></div>
  </div>
</div>

<!-- CONFIRM MODAL -->
<div class="modal" id="confirmModal" style="z-index:95">
  <div class="modal-box">
    <h3 id="confirmTitle">Confirmar</h3>
    <p id="confirmMsg" style="font-size:13.5px;color:#e3dcff"></p>
    <div class="btnrow"><button class="btn" id="confirmYes">Confirmar</button><button class="btn sec" id="confirmNo">Cancelar</button></div>
  </div>
</div>

<!-- LIGHTBOX -->
<div class="lightbox" id="lightbox">
  <button class="lbnav prev" id="lbPrev">‹</button>
  <button class="lbnav next" id="lbNext">›</button>
  <img id="lbImg" src="" alt="">
  <div class="lbpos" id="lbPos"></div>
  <div class="lbcompliment" id="lbCompliment"></div>
  <div class="lbinfo" id="lbInfo"></div>
  <textarea id="lbCaption" placeholder="Escreva a descrição desta foto... pode usar parágrafos e quebras de linha."></textarea>
  <div class="btnrow lbtns"><button class="btn" id="lbSave">💾 Salvar</button><button class="btn sec" id="lbDelete">🗑️ Apagar</button><button class="btn sec" id="lbClose">Fechar</button></div>
</div>

<script>
try{var _v=document.getElementById('vstamp');if(_v)_v.textContent='versão 13 · ativo ✓';}catch(e){}
/* $on(id): acesso seguro a elementos. Elemento real passa direto; se faltar, devolve um stub inofensivo (nunca derruba o script). */
function $on(id){var e=document.getElementById(id);if(e)return e;var noop=function(){};return new Proxy({},{get:function(t,p){
  if(p==='classList')return {add:noop,remove:noop,toggle:noop,contains:function(){return false;}};
  if(p==='style'||p==='dataset')return {};
  if(p==='value'||p==='textContent'||p==='innerHTML'||p==='src'||p==='href'||p==='title')return '';
  if(p==='files')return [];
  if(p==='checked')return false;
  if(p==='querySelectorAll')return function(){return [];};
  if(p==='querySelector'||p==='closest')return function(){return null;};
  if(p==='getAttribute')return function(){return null;};
  return noop;
},set:function(){return true;}});}
/* Entrada garantida: definida no topo, usa funcoes hasteadas (hoisted) */
try{window.activateTab=activateTab;}catch(e){}
try{window.reRenderAll=reRenderAll;}catch(e){}
window.__enterApp=function(go){
  go=go||'mem';
  try{var g=$on('guestName');var nm=(window.__splashSel==='__guest')?((g&&g.value||'').trim()||'Convidado'):window.__splashSel;if(nm)localStorage.setItem('username',nm);}catch(e){}
  try{if(typeof refreshWhoChip==='function')refreshWhoChip();}catch(e){}
  try{if(typeof reRenderAll==='function')reRenderAll();}catch(e){}
  var sp=$on('splash');if(sp)sp.classList.add('hide');
  try{if(typeof activateTab==='function')activateTab(go);}catch(e){}
};
/* Navegacao a prova de falhas: delegacao no documento (funciona mesmo se a parte de baixo do script falhar) */
document.addEventListener('click',function(e){
  if(!e.target||!e.target.closest)return;
  var t=function(sel){return e.target.closest(sel);};var el;
  try{
    if((el=t('.tab'))){if(typeof activateTab==='function')activateTab(el.getAttribute('data-tab')||el.getAttribute('data-go'));return;}
    if(t('#toggleBtn')){if(typeof activateTab==='function')activateTab(document.body.classList.contains('mem')?'d1':'mem');return;}
    if(t('#homeBtn')){if(typeof appConfirm==='function')appConfirm('Voltar à tela inicial?',openSplash);else if(typeof openSplash==='function')openSplash();return;}
    if(t('#fabAdd')){if(typeof activateTab==='function')activateTab('mem');var mf=$on('mform');mf.classList.add('open');try{mf.scrollIntoView({behavior:'smooth',block:'start'});}catch(_){}return;}
    if(t('#dedHeart')){$on('dedModal').classList.add('open');return;}
    if(t('#dedClose')){$on('dedModal').classList.remove('open');return;}
    if(t('#syncTopBtn')){$on('syncModal').classList.add('open');return;}
    if(t('#syncClose')){$on('syncModal').classList.remove('open');return;}
    if(t('#splashGear')){$on('gearModal').classList.add('open');return;}
    if(t('#gearClose')){$on('gearModal').classList.remove('open');return;}
    if(t('#modalClose')){$on('modal').classList.remove('open');return;}
    if(t('#choosePlace')){window.placePickCb=null;if(typeof resetPlaceList==='function')resetPlaceList();$on('placeModal').classList.add('open');return;}
    if(t('#placeClose')){$on('placeModal').classList.remove('open');window.placePickCb=null;return;}
    if(t('#mformHead')){$on('mform').classList.toggle('open');return;}
    if(t('#expandAll')){document.querySelectorAll('#momentsList .moment').forEach(function(m){m.classList.add('open');});return;}
    if(t('#collapseAll')){document.querySelectorAll('#momentsList .moment').forEach(function(m){m.classList.remove('open');});return;}
    if(t('#splashGuide')){var nm=window.__splashSel;if(nm==='__guest')nm=($on('guestName').value||'').trim()||'Convidado';try{if(nm)localStorage.setItem('username',nm);}catch(_){}try{if(typeof refreshWhoChip==='function')refreshWhoChip();}catch(_){}try{if(typeof reRenderAll==='function')reRenderAll();}catch(_){}$on('splash').classList.add('hide');if(typeof activateTab==='function')activateTab('d1');return;}
  }catch(err){}
});
const MAP={metro:"https://www.google.com/maps/search/?api=1&query=Mairie%20de%20Montrouge&query_place_id=ChIJQVV_yapx5kcR0Q-hLHu4bCk",adventure:"https://www.google.com/maps/search/?api=1&query=Disney%20Adventure%20World%20Chessy&query_place_id=ChIJ_YETR4Ad5kcRyKP2sKsvtSE",disneyland:"https://www.google.com/maps/search/?api=1&query=Disneyland%20Park%20Paris&query_place_id=ChIJf9hphiUd5kcR5RdeomHtvFA",primark:"https://www.google.com/maps/search/?api=1&query=Primark%20Val%20d%27Europe&query_place_id=ChIJPXYiDbkd5kcRUNIX6Bq2tlc"};

const DIA1=[
  {t:"~08:30",e:"🚇",n:"Saímos do hotel direto pro Primark",z:"Metrô 4 + RER A",b:"info",special:true,map:MAP.metro,maplabel:"Abrir estação no mapa",d:"Acabamos pegando o trem errado e nos atrasamos, então fomos direto para o Primark, que abre às 11h, e almoçamos no shopping antes de entrar no parque.",howsteps:["Na estação Mairie de Montrouge, pegamos o Metrô Linha 4 na direção Porte de Clignancourt.","Descemos na estação Nation.","Em Nation, pegamos o RER A e fomos até Val d'Europe, onde fica o Primark."]},
  {t:"11:00",e:"🛍️",n:"Primark no Val d'Europe",z:"Compras e almoço",b:"info",special:true,map:MAP.primark,maplabel:"Abrir Primark no mapa",d:"A loja abre às 11h. Fizemos as compras e almoçamos no shopping com calma antes de ir para o parque.",how:"De Val d'Europe, pegamos o RER A uma parada até a Disney, na estação Marne la Vallée Chessy."},
  {t:"13:30",e:"🎟️",n:"Chegamos no parque",z:"Disney Adventure World",b:"info",special:true,map:MAP.adventure,maplabel:"Abrir parque no mapa",d:"Entramos às 13h30, já almoçados. À tarde as filas das principais ficam maiores, então fomos direto nelas.",how:"Procuramos a placa Single Rider nas atrações mais concorridas para adiantar a fila."},
  {t:"13:30",e:"🐢",n:"Crush's Coaster",z:"World of Pixar",b:"g",tags:[["must","Imperdível"],["kid","Maria amou"]],d:"A montanha-russa do Nemo, gira dentro de uma concha de tartaruga pelo escuro. Divertida e sem ser assustadora.",how:"Encaramos os 100 minutos de fila e valeu a pena! É a mais concorrida do parque."},
  {t:"15:20",e:"🏎️",n:"RC Racer",z:"World of Pixar",b:"y",tags:[["must","Imperdível"]],d:"Mistura de autorama com barco viking, sobe e desce num trilho em U bem alto.",how:"Ficamos cerca de 30 minutos na fila. É rápida e divertida."},
  {t:"16:00",e:"🐭",n:"Ratatouille",z:"World of Pixar",b:"g",tags:[["must","Imperdível"]],d:"Simulador em quatro dimensões pela cozinha do Remy. Favorita das famílias, sem altura nem queda.",how:"Ficamos 80 minutos na fila e valeu a pena. Viemos direto do RC Racer para cá."},
  {t:"17:30",e:"❄️",n:"Frozen Ever After",z:"World of Frozen",b:"g",tags:[["must","Imperdível"],["kid","Maria amou"]],d:"Passeio de barco pela história do Frozen, com a Elsa e a Anna. Encantador e tranquilo.",how:"Ficamos 75 minutos na fila. Área nova e linda, aproveitamos para tirar muitas fotos."},
  {t:"18:50",e:"🚗",n:"Cars Road Trip",z:"Cars Route 66",b:"g",tags:[["kid","Tranquila"]],d:"Um passeio tranquilo com os carros do filme Cars por uma estrada cênica. Calmo e divertido.",how:"Ficamos só 10 minutos na fila."},
  {t:"19:10",e:"🕷️",n:"Spider-Man Web Adventure",z:"Avengers Campus",b:"g",tags:[["kid","Maria amou"]],d:"Atração interativa em que lançamos teias com os braços para ajudar o Homem-Aranha. Todo mundo curtiu e não tem radicalismo.",how:"Achamos ela e ficamos só 15 minutos na fila."},
  {t:"19:35",e:"🦸",n:"Avengers Assemble: Flight Force",z:"Avengers Campus",b:"r",finale:true,tags:[["must","A última do dia"]],d:"A montanha-russa mais radical do parque, acelera forte e tem inversões. Tema da Marvel.",how:"Foi a última do dia e ficamos só 10 minutos na fila. Fechou com adrenalina!"},
  {t:"22:30",e:"🏡",n:"Chegamos em casa",z:"Fim do Dia 1",b:"info",special:true,d:"Voltamos para o hotel por volta das 22h30, cansados e muito felizes depois de um dia incrível na Disney.",how:"Que dia! Amanhã tem o Disneyland Park."},
];
const DIA2=[
  {t:"07:45",e:"🚇",n:"Sair do hotel",z:"Metrô 4 até o RER A",b:"info",special:true,map:MAP.metro,maplabel:"Abrir estação no mapa",d:"Mesmo trajeto do Dia 1, cerca de 55 minutos. Saindo às 7h45 vocês chegam por volta das 9h. Comprem algo rápido no caminho.",howsteps:["Na estação Mairie de Montrouge, peguem o Metrô Linha 4 na direção Porte de Clignancourt.","Desçam na estação Nation.","Em Nation, peguem o RER A na direção Marne la Vallée Chessy e fiquem até a última estação."]},
  {t:"09:00",e:"🎟️",n:"Chegamos no parque",z:"Entrada, esperando abrir",b:"info",special:true,map:MAP.disneyland,maplabel:"Abrir parque no mapa",d:"O parque abre às 9h30. Cheguem por volta das 9h e fiquem pertinho do portão.",how:"Deixem os ingressos já abertos no celular."},
  {t:"09:35",e:"🚀",n:"Star Wars Hyperspace Mountain",z:"Discoveryland",b:"y",tags:[["must","A melhor"]],d:"É uma montanha-russa no escuro com tema de Star Wars, considerada a melhor Space Mountain do mundo. É rápida e tem loopings.",how:"Tem a pior fila do parque, então corram direto para cá ao abrir. Você e a Maria topam, e vale conferir com a Thaysa."},
  {t:"10:15",e:"🎯",n:"Buzz Lightyear Laser Blast",z:"Discoveryland",b:"g",tags:[["must","Imperdível"],["kid","Competição em família"]],d:"É um carrinho com pistolas laser. Vence quem fizer mais pontos acertando os alvos. Rende uma boa disputa entre vocês.",how:"É calma e divertida. Façam logo depois da Hyperspace."},
  {t:"10:55",e:"🛸",n:"Star Tours",z:"Discoveryland",b:"g",tags:[["kid","Se der tempo"]],d:"É um simulador em três dimensões pela galáxia de Star Wars. É tranquilo, só balança um pouco.",how:"Façam se a fila estiver curta antes da parada."},
  {t:"11:30",e:"🎠",n:"Disney Stars on Parade",z:"Central Plaza, parada",b:"g",finale:true,tags:[["show","Parada do dia"]],d:"É a grande parada que percorre a Main Street com carros alegóricos e personagens. É bem mágica.",how:"Peguem lugar na Central Plaza uns 15 minutos antes e confirmem o horário no app."},
  {t:"12:00",e:"🏰",n:"Castelo e Toca do Dragão",z:"Fantasyland",b:"g",tags:[["must","Imperdível"],["kid","Maria vai amar"]],d:"É o Castelo da Bela Adormecida. Dá para explorar por dentro, com vitrais e murais, e descer na Toca do Dragão, uma passagem secreta que só existe na Disney de Paris.",how:"Não costuma ter fila grande. As fotos aqui ficam lindas."},
  {t:"12:40",e:"🧚",n:"Peter Pan's Flight",z:"Fantasyland",b:"g",tags:[["kid","Clássico"]],d:"É um voo sobre a Terra do Nunca num barquinho voador. É um clássico da Disney, simples e gostoso.",how:"Costuma ter fila, então façam agora que já estão na Fantasyland."},
  {t:"13:15",e:"🃏",n:"Alice's Curious Labyrinth",z:"Fantasyland",b:"g",tags:[["kid","Maria vai amar"]],d:"É um labirinto com tema de Alice no País das Maravilhas. As crianças, e a Maria também, adoram.",how:"É uma diversão para explorar com calma."},
  {t:"13:45",e:"🍕",n:"Almoço na Pizzeria Bella Notte",z:"Fantasyland",b:"info",special:true,d:"É um restaurante com tema de A Dama e o Vagabundo, que serve pizzas e massas. Já fica aqui na Fantasyland, então não tem deslocamento.",how:"Recarreguem as energias antes de seguir para a Frontierland. Confiram no app se tem algum item em formato do Mickey."},
  {t:"14:45",e:"🏔️",n:"Big Thunder Mountain",z:"Frontierland",b:"g",tags:[["must","Imperdível"]],d:"É uma montanha-russa de madeira numa ilha. É veloz e divertida, mas não tem loopings, então todo mundo encara.",how:"É uma das melhores e mais acessíveis, e costuma ser a favorita da família toda."},
  {t:"15:25",e:"👻",n:"Phantom Manor",z:"Frontierland",b:"y",tags:[["must","Imperdível"]],d:"É a casa mal-assombrada da Disney de Paris. A atmosfera é sombria e assusta um pouquinho, mas é mais charme do que susto.",how:"Se a Maria topar um terror leve, vão. É muito bem produzida."},
  {t:"16:10",e:"🪨",n:"Indiana Jones",z:"Adventureland",b:"y",tags:[["must","Imperdível"]],d:"É a montanha-russa do Indiana Jones e tem uma volta de 360 graus. É curtinha e intensa.",how:"Confiram a altura mínima na entrada."},
  {t:"16:50",e:"☠️",n:"Pirates of the Caribbean",z:"Adventureland",b:"g",tags:[["must","Imperdível"]],d:"É um barco que navega pela história dos Piratas do Caribe, com cenários incríveis. É calmo e imperdível.",how:"Fecha bem a volta do parque. A família toda adora."},
  {t:"Noite",e:"🎆",n:"Disney Tales of Magic",z:"Castelo, encerramento",b:"g",finale:true,tags:[["show","Grande final"]],d:"É o show noturno, com projeções no castelo, fontes e fogos. É o momento mais mágico do dia.",how:"Peguem lugar de frente para o castelo uns 30 minutos antes e não percam por nada."},
];

const DEDICATION="Esta viagem pela Europa foi um sonho que vivemos de mãos dadas. De Paris a Amsterdam, passando por Bruxelas e Bruges, cada rua, cada canal e cada luz que se acendeu no céu ganhou mais cor porque estávamos juntos. O Lilo não pôde vir, mas esteve em cada saudade boa e em cada pensamento nosso. Aqui ficam guardados os risos, os abraços, o cansaço gostoso no fim do dia e aquele aperto no peito de pura felicidade. Que sempre que abrirmos este álbum, a gente volte a sentir tudo de novo. Porque lugares a gente visita, mas momentos como estes ficam para sempre.";
const COMPLIMENTS=["Que momento lindo!","Puro encanto!","Isso é inesquecível!","Que cena maravilhosa!","Guardado para sempre!","Que recordação especial!","Simplesmente perfeito!","Que vista incrível!","Momento de ouro!","Que registro lindo!","Pura magia!","Que dia especial!","Isso vale uma moldura!","Que felicidade guardada aqui!","Lindo demais!","Que instante mágico!","Memória para a vida toda!","Que cenário maravilhoso!","Puro brilho!","Que clique perfeito!","Isso é a Eurotrip em uma foto!","Que momento de cinema!","Inesquecível!","Que beleza!","Aqui mora uma boa lembrança!","Que paisagem de tirar o fôlego!","Puro amor neste momento!","Que registro precioso!","Isso ficou maravilhoso!","Que recordação de ouro!","Momento mágico da viagem!","Que foto cheia de vida!","Guardando esse instante com carinho!","Que cena encantadora!","Puro charme!","Que lembrança linda da viagem!","Isso é felicidade!","Que vista de cartão-postal!","Momento perfeito!","Que dia para nunca esquecer!","Pura beleza!","Que registro cheio de alegria!","Isso merece destaque!","Que instante especial!","Linda recordação!","Que cena para guardar no coração!","Puro encanto da viagem!","Que momento radiante!","Aqui tem história!","Que lembrança maravilhosa!"];
function toast(msg){let t=$on('toast');if(!t){t=document.createElement('div');t.id='toast';document.body.appendChild(t);}t.textContent=msg;t.classList.add('show');clearTimeout(window.__toastT);window.__toastT=setTimeout(()=>t.classList.remove('show'),1800);}

const PEOPLE=["Edson","Maria","Thaysa"];
const DISNEY_PLACES=["Disneyland Park","Disney Adventure World","Main Street USA","Castelo da Bela Adormecida","Toca do Dragão","Pizzeria Bella Notte","Loja da Disney","Primark Val d'Europe"];
const PARIS_PLACES=["Torre Eiffel","Arco do Triunfo","Museu do Louvre","Catedral de Notre-Dame","Montmartre","Basílica de Sacré-Cœur","Avenida Champs-Élysées","Rio Sena","Jardim de Luxemburgo","Ópera Garnier","Galeries Lafayette","Trocadéro","Ponte Alexandre III","Bairro Latino","Moulin Rouge","Hotel em Paris","Restaurante em Paris"];
const BRUXELAS_PLACES=["Grand Place de Bruxelas","Atomium","Manneken Pis","Galerias Saint-Hubert","Parque do Cinquantenário","Catedral de Bruxelas","Restaurante em Bruxelas"];
const BRUGES_PLACES=["Centro histórico de Bruges","Canais de Bruges","Praça Markt","Campanário Belfort","Lago do Amor (Minnewater)","Igreja de Nossa Senhora"];
const AMSTERDAM_PLACES=["Canais de Amsterdam","Museu Van Gogh","Rijksmuseum","Casa de Anne Frank","Praça Dam","Vondelpark","Bairro Jordaan","Mercado de Flores"];
const GERAL_PLACES=["Trem / Eurostar","Hotel","Restaurante","Outro lugar"];
let KNOWN_PLACES=new Set();
const GENERIC_PLACES=new Set(["Outro lugar","Fila de uma atração","Hotel","Restaurante","Trem / Eurostar","Loja da Disney","Entrada do parque","Hotel em Paris","Restaurante em Paris","Restaurante em Bruxelas","Praça central do castelo"]);
function isLinkablePlace(p){return KNOWN_PLACES.has(p)&&!GENERIC_PLACES.has(p);}
function mapsUrl(p){return 'https://www.google.com/maps/search/?api=1&query='+encodeURIComponent(p);}
function authorChip(name){if(!name)return '';const ph=getProfile(name);const av=ph?`<span class="achip-av"><img src="${ph}"></span>`:'<span class="achip-av">👤</span>';return `<span class="authchip">${av}${name}</span>`;}
function placePill(place){if(!place)return '';const cls=placeClass(place);if(isLinkablePlace(place)){return `<a class="mplace ${cls}" href="${mapsUrl(place)}" target="_blank" rel="noopener">📍 ${place}</a>`;}return `<span class="mplace ${cls}">📍 ${place}</span>`;}
function photoRowsAlbum(key){const photos=getPhotos(key);return photos.map((p,idx)=>`<div class="photorow${p.caption?'':' nocap'}"><div class="thumb"><img src="${p.src}" data-key="${key}" data-idx="${idx}" class="viewphoto">${p.caption?'<span class="cap-dot">📝</span>':''}</div>${p.caption?`<div class="prcap">${escHtml(p.caption)}</div>`:''}</div>`).join('');}

const store={get(k){try{return localStorage.getItem(k);}catch(e){return (window.__mem||{})[k]??null;}},set(k,v){try{localStorage.setItem(k,v);return true;}catch(e){(window.__mem=window.__mem||{})[k]=v;return false;}},del(k){try{localStorage.removeItem(k);}catch(e){if(window.__mem)delete window.__mem[k];}},keys(){try{return Object.keys(localStorage);}catch(e){return Object.keys(window.__mem||{});}}};

function userName(){return store.get('username')||'Família';}
function nowTs(){return Date.now();}
function getProfile(name){return store.get('profile_'+name)||'';}
function setProfile(name,d){store.set('profile_'+name,d);}
function dmy(d){if(!d)return '';const p=d.split('-');return p.length===3?p[2]+'/'+p[1]+'/'+p[0]:d;}
function fmtDateOnly(ts){try{return new Date(ts).toLocaleDateString('pt-BR');}catch(e){return '';}}
const confirmModal=$on('confirmModal');let confirmCb=null;
function appConfirm(msg,cb){$on('confirmTitle').textContent='Confirmar';$on('confirmNo').style.display='';$on('confirmMsg').textContent=msg;confirmCb=cb;confirmModal.classList.add('open');}
function appNotice(msg){$on('confirmTitle').textContent='Aviso';$on('confirmNo').style.display='none';$on('confirmMsg').textContent=msg;confirmCb=null;confirmModal.classList.add('open');}
$on('confirmYes').addEventListener('click',()=>{confirmModal.classList.remove('open');const cb=confirmCb;confirmCb=null;if(cb)cb();});
$on('confirmNo').addEventListener('click',()=>{confirmModal.classList.remove('open');confirmCb=null;});

function getPhotos(key){const v=store.get('ph_'+key);if(!v)return [];try{return JSON.parse(v).map(p=>typeof p==='string'?{src:p,author:'',ts:0}:p);}catch(e){return [];}}
function setPhotos(key,arr){const ok=store.set('ph_'+key,JSON.stringify(arr));if(!ok&&arr.length){alert('Não consegui salvar a foto, o espaço do navegador pode estar cheio. Abra a engrenagem e copie o site completo para guardar tudo no GitHub.');}}

function resizeBlob(blob){return new Promise((resolve,reject)=>{const url=URL.createObjectURL(blob);const img=new Image();img.onload=()=>{URL.revokeObjectURL(url);const maxDim=1000;let w=img.width,h=img.height;if(w>h){if(w>maxDim){h=Math.round(h*maxDim/w);w=maxDim;}}else{if(h>maxDim){w=Math.round(w*maxDim/h);h=maxDim;}}const c=document.createElement('canvas');c.width=w;c.height=h;c.getContext('2d').drawImage(img,0,0,w,h);try{resolve(c.toDataURL('image/jpeg',0.58));}catch(e){reject(e);}};img.onerror=()=>{URL.revokeObjectURL(url);reject(new Error('load'));};img.src=url;});}
async function processImage(file){const isHeic=/heic|heif/i.test(file.type)||/\.hei[cf]$/i.test(file.name);let blob=file;if(isHeic&&window.heic2any){try{const out=await window.heic2any({blob:file,toType:'image/jpeg',quality:0.85});blob=Array.isArray(out)?out[0]:out;}catch(e){}}return await resizeBlob(blob);}

function tagHTML(tags){if(!tags)return '';return tags.map(([c,t])=>`<span class="tag ${c}">${t}</span>`).join('');}
function badgeClass(b){return {g:'d-g',y:'d-y',r:'d-r'}[b]||'';}
function escHtml(t){return (t||'').replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;');}
function photoThumbs(key){const photos=getPhotos(key);return photos.map((p,idx)=>`<div class="thumb"><img src="${p.src}" data-key="${key}" data-idx="${idx}" class="viewphoto">${p.caption?'<span class="cap-dot">📝</span>':''}</div>`).join('');}
function photoBlock(key){return `<div class="photobox"><div class="pl">📷 Fotos (toque para ver a descrição)</div><div class="thumbs">${photoThumbs(key)}<label class="addphoto"><span>＋</span>foto<input type="file" accept="image/*" class="photoinput" multiple data-key="${key}"></label></div></div>`;}

function render(list,mountId,dayKey){
  const tl=$on(mountId);
  tl.innerHTML=list.map((it,i)=>{
    const key=dayKey+'_'+i;const done=store.get(key)==='1';
    const showBadge=['g','y','r'].includes(it.b);const extraCls=(it.special?' special':'')+(it.finale?' finale':'');
    const checkBtn=showBadge?`<div class="check" data-key="${key}">✓</div>`:'';
    let howHTML='';if(it.howsteps){howHTML=`<div class="howto"><b>Passo a passo:</b><ol>${it.howsteps.map(s=>`<li>${s}</li>`).join('')}</ol></div>`;}else if(it.how){howHTML=`<div class="howto"><b>Como fazer:</b> ${it.how}</div>`;}
    const mapHTML=it.map?`<a class="maplink" href="${it.map}" target="_blank">📍 ${it.maplabel||'Abrir no mapa'}</a>`:'';
    return `<div class="item"><div class="card${done?' done':''}${extraCls}" style="animation-delay:${i*0.05}s"><div class="chead" data-toggle><span class="emoji">${it.e}</span><span class="ctitle"><b>${it.n}</b><span class="zone">${it.z}</span></span>${showBadge?`<span class="badge ${badgeClass(it.b)}"></span>`:''}${checkBtn}<span class="chev">▼</span></div><div class="cbody"><div class="cbody-in"><div class="timeline-time">🕐 Horário sugerido: ${it.t}</div>${tagHTML(it.tags)}<p>${it.d}</p>${howHTML}${mapHTML}</div></div></div></div>`;
  }).join('');
  bindCards(tl);
}
function bindCards(root){
  root.querySelectorAll('.chead[data-toggle]').forEach(h=>{h.addEventListener('click',e=>{if(e.target.closest('.check'))return;h.closest('.card').classList.toggle('open');});});
  root.querySelectorAll('.check').forEach(c=>{c.addEventListener('click',e=>{e.stopPropagation();const k=c.dataset.key,card=c.closest('.card');const now=!card.classList.contains('done');card.classList.toggle('done',now);store.set(k,now?'1':'0');});});
  root.querySelectorAll('.photoinput').forEach(inp=>{inp.addEventListener('change',async e=>{const files=[...e.target.files];if(!files.length)return;const key=inp.dataset.key;const arr=getPhotos(key);let ok=0;for(const file of files){try{const data=await processImage(file);arr.push({src:data,author:userName(),ts:nowTs()});ok++;}catch(err){}}setPhotos(key,arr);reRenderAll();if(ok)toast(ok>1?(ok+' fotos adicionadas 📷'):'Foto adicionada 📷');});});
  root.querySelectorAll('.viewphoto').forEach(img=>{img.addEventListener('click',e=>{e.stopPropagation();openLightbox(img.dataset.key,parseInt(img.dataset.idx));});});
}
function reRenderAll(){render(DIA1,'tl-d1','d1');render(DIA2,'tl-d2','d2');renderMoments();updateCounts();renderAlbum();}

let lbKey=null,lbIdx=null;const lightbox=$on('lightbox');
function openLightbox(key,idx){lbKey=key;lbIdx=idx;const arr=getPhotos(key);const p=arr[idx];if(!p)return;$on('lbImg').src=p.src;$on('lbInfo').textContent=(p.ts?fmtDateOnly(p.ts):'');$on('lbCaption').value=p.caption||'';$on('lbCompliment').textContent='💛 '+COMPLIMENTS[Math.floor(Math.random()*COMPLIMENTS.length)];$on('lbPos').textContent=arr.length>1?((idx+1)+' / '+arr.length):'';$on('lbPrev').style.display=arr.length>1?'flex':'none';$on('lbNext').style.display=arr.length>1?'flex':'none';lightbox.classList.add('open');}
function lbNav(delta){saveCaption();const arr=getPhotos(lbKey);if(!arr.length)return;let i=lbIdx+delta;if(i<0)i=arr.length-1;if(i>=arr.length)i=0;openLightbox(lbKey,i);}
function saveCaption(){const arr=getPhotos(lbKey);if(arr[lbIdx]){arr[lbIdx].caption=$on('lbCaption').value;setPhotos(lbKey,arr);}}
function closeLightbox(){saveCaption();lightbox.classList.remove('open');reRenderAll();}
$on('lbClose').addEventListener('click',closeLightbox);
$on('lbSave').addEventListener('click',()=>{saveCaption();lightbox.classList.remove('open');reRenderAll();toast('Descrição salva 💛');});
$on('lbDelete').addEventListener('click',()=>{appConfirm('Apagar esta foto?',()=>{const photos=getPhotos(lbKey);photos.splice(lbIdx,1);setPhotos(lbKey,photos);lightbox.classList.remove('open');reRenderAll();});});
$on('lbPrev').addEventListener('click',()=>lbNav(-1));
$on('lbNext').addEventListener('click',()=>lbNav(1));
(function(){var lb=$on('lbImg');if(!lb)return;let x0=null;lb.addEventListener('touchstart',e=>{x0=e.touches[0].clientX;},{passive:true});lb.addEventListener('touchend',e=>{if(x0===null)return;const dx=e.changedTouches[0].clientX-x0;if(Math.abs(dx)>50)lbNav(dx<0?1:-1);x0=null;},{passive:true});})();

function placeClass(p){p=(p||'').toLowerCase();
  if(/disney|castelo|drag|pixar|frozen|avenger|spider|crush|ratatouille|tower|mountain|pirate|peter|alice|buzz|star tours|indiana|bella notte|main street|hyperspace|arendelle|raiponce/.test(p))return 'pc-disney';
  if(/paris|torre|eiffel|louvre|arco|sena|montmartre|champs|notre|trocad|opera|lafayette|moulin|latino|alexandre/.test(p))return 'pc-paris';
  if(/bruxelas|grand place|atomium|manneken|cinquenten|saint-hubert/.test(p))return 'pc-bx';
  if(/bruges|markt|belfort|minnewater|nossa senhora/.test(p))return 'pc-bg';
  if(/amsterd|van gogh|rijks|anne frank|dam|vondel|jordaan|flores/.test(p))return 'pc-ams';
  return 'pc-def';
}
const TRIP_DAYS=[];(function(){for(let d=4;d<=15;d++){TRIP_DAYS.push('2026-06-'+String(d).padStart(2,'0'));}})();
function dayNum(date){return date?String(parseInt(date.split('-')[2],10)):'';}
function migrateMoment(m){if(!m.places)m.places=m.place?[m.place]:[];if(!m.dates)m.dates=m.date?[m.date]:[];return m;}
function momentDates(m){return (m.dates&&m.dates.length)?m.dates.slice().sort():(m.date?[m.date]:[]);}
function momentPlaces(m){return (m.places&&m.places.length)?m.places:(m.place?[m.place]:[]);}
const MON_ABBR=['jan','fev','mar','abr','mai','jun','jul','ago','set','out','nov','dez'];
function monOf(date){return MON_ABBR[parseInt(date.split('-')[1],10)-1];}
function datesSummary(m){const ds=momentDates(m);if(!ds.length)return '';if(ds.length===1)return '📅 '+dayNum(ds[0])+' '+monOf(ds[0]);const a=ds[0],b=ds[ds.length-1];if(monOf(a)===monOf(b))return '📅 '+dayNum(a)+'–'+dayNum(b)+' '+monOf(a);return '📅 '+dayNum(a)+' '+monOf(a)+'–'+dayNum(b)+' '+monOf(b);}
function placesSummary(m){const ps=momentPlaces(m);if(!ps.length)return '';if(ps.length===1)return placePill(ps[0]);return `<span class="mplace pc-def">📍 ${ps.length} locais</span>`;}
function placesPills(m){return momentPlaces(m).map(p=>placePill(p)).join(' ');}
function getMoments(){const v=store.get('moments');if(!v)return [];try{return JSON.parse(v).map(migrateMoment);}catch(e){return [];}}
function setMoments(arr){store.set('moments',JSON.stringify(arr));}
let formPhotos=[];
function renderFormPhotos(){const c=$on('formPhotos');c.innerHTML=formPhotos.map((p,i)=>`<div class="thumb"><img src="${p.src}" data-capidx="${i}" class="formcap">${p.caption?'<span class="cap-dot">📝</span>':''}<span class="who-badge" data-rm="${i}">✕ tirar</span></div>`).join('');c.querySelectorAll('[data-rm]').forEach(b=>b.addEventListener('click',e=>{e.stopPropagation();formPhotos.splice(b.dataset.rm,1);renderFormPhotos();}));c.querySelectorAll('.formcap').forEach(img=>img.addEventListener('click',()=>openCapModal(parseInt(img.dataset.capidx))));}
let capIdx=null;
function openCapModal(i){capIdx=i;$on('capImg').src=formPhotos[i].src;$on('capText').value=formPhotos[i].caption||'';$on('capModal').classList.add('open');}
let formPlaces=[];let formDaysSet=new Set();let diaryDaysSet=new Set();let albumDaysSet=new Set();
function renderFormPlaces(){const c=$on('formPlaces');c.innerHTML=formPlaces.map((p,i)=>`<span class="selchip">${p}<b data-rmp="${i}">✕</b></span>`).join('');c.querySelectorAll('[data-rmp]').forEach(b=>b.addEventListener('click',()=>{formPlaces.splice(b.dataset.rmp,1);renderFormPlaces();}));}
function addFormPlace(v){v=(v||'').trim();if(!v)return;if(!formPlaces.includes(v))formPlaces.push(v);renderFormPlaces();}
let pickerTarget=null,pickerCb=null,pStart=null,pEnd=null;
function daysLabel(set,emptyText){const arr=[...set].sort();if(!arr.length)return emptyText;if(arr.length===1)return '📅 '+dayNum(arr[0])+' jun';return '📅 '+dayNum(arr[0])+' a '+dayNum(arr[arr.length-1])+' jun';}
function updateDaysBtn(id,set,emptyText){const b=$on(id);if(b)b.textContent=daysLabel(set,emptyText);}
function renderFormDays(){updateDaysBtn('formDaysBtn',formDaysSet,'📅 Escolher dias');}
function renderDayPicker(){const c=$on('dayPicker');c.innerHTML=TRIP_DAYS.map(d=>{let on=false;if(pStart&&pEnd){on=(d>=pStart&&d<=pEnd);}else if(pStart){on=(d===pStart);}return `<button class="daychip${on?' on':''}" data-day="${d}">${dayNum(d)}</button>`;}).join('');c.querySelectorAll('[data-day]').forEach(b=>b.addEventListener('click',()=>{const d=b.dataset.day;if(pStart&&!pEnd&&d===pStart){pStart=null;}else if(!pStart||(pStart&&pEnd)){pStart=d;pEnd=null;}else{if(d<pStart){pEnd=pStart;pStart=d;}else{pEnd=d;}}renderDayPicker();}));}
function openDayPicker(targetSet,cb){pickerTarget=targetSet;pickerCb=cb;const arr=[...targetSet].sort();pStart=arr[0]||null;pEnd=arr.length?arr[arr.length-1]:null;renderDayPicker();$on('dayModal').classList.add('open');}
$on('mPhotoInput').addEventListener('change',async e=>{const files=[...e.target.files];if(!files.length)return;let ok=0;for(const file of files){try{const data=await processImage(file);formPhotos.push({src:data,author:userName(),ts:nowTs()});ok++;}catch(err){}}renderFormPhotos();if(ok)toast(ok>1?(ok+' fotos adicionadas 📷'):'Foto adicionada 📷');e.target.value='';});

function momentKey(m){const ds=momentDates(m);if(ds.length)return new Date(ds[0]+'T00:00:00').getTime();return m.ts||0;}
function photoViewBlock(key){const t=photoThumbs(key);if(!t)return '';return `<div class="photobox"><div class="pl">📷 Fotos (toque para ver)</div><div class="thumbs">${t}</div></div>`;}
let editState={title:'',note:'',places:[],dates:new Set()};
function resetPlaceList(){document.querySelectorAll('#placeList [data-place]').forEach(b=>{b.classList.remove('picked');b.textContent=b.dataset.place;});}
function inlineEditorHTML(m){
  const photos=getPhotos('m'+m.id);
  const thumbs=photos.map((p,idx)=>`<div class="thumb"><img src="${p.src}" data-key="m${m.id}" data-idx="${idx}" class="viewphoto">${p.caption?'<span class="cap-dot">📝</span>':''}<span class="who-badge ie-rmphoto" data-key="m${m.id}" data-idx="${idx}">✕</span></div>`).join('');
  return `<div class="ineditor">
    <input class="ie-input ie-title" value="${(editState.title||'').replace(/"/g,'&quot;')}" placeholder="Título">
    <div class="fflabel2">📍 Locais</div>
    <div class="placewrap"><input class="ie-input ie-place" placeholder="Digite ou escolha..."><button class="choosebtn ie-addplace">+</button><button class="choosebtn ie-listplace">📍 Lista</button></div>
    <div class="chipsel ie-places">${editState.places.map((p,i)=>`<span class="selchip">${p}<b data-iep="${i}">✕</b></span>`).join('')}</div>
    <div class="fflabel2">📅 Dias</div>
    <button class="btn sec tiny ie-daysbtn" style="width:auto;margin-bottom:10px">${daysLabel(editState.dates,'📅 Escolher dias')}</button>
    <textarea class="ie-input ie-note" rows="2" placeholder="Descrição">${escHtml(editState.note||'')}</textarea>
    <div class="photobox"><div class="pl">📷 Fotos</div><div class="thumbs">${thumbs}<label class="addphoto"><span>＋</span>foto<input type="file" accept="image/*" class="ie-addphoto" multiple data-key="m${m.id}"></label></div></div>
    <div class="btnrow"><button class="btn ie-save">💾 Salvar</button><button class="btn sec ie-cancel">Cancelar</button></div>
  </div>`;
}
function renderMoments(){
  const list=$on('momentsList');
  let moments=getMoments().slice().sort((a,b)=>momentKey(a)-momentKey(b));
  if(diaryDaysSet.size){moments=moments.filter(m=>momentDates(m).some(d=>diaryDaysSet.has(d)));}
  if(!moments.length){list.innerHTML='<div class="empty">'+(diaryDaysSet.size?'Nenhum momento nesse(s) dia(s).':'Ainda não há momentos. Que tal registrar a primeira lembrança da viagem?')+'</div>';return;}
  list.innerHTML=moments.map((m)=>{
    const editing=(String(editingId)===String(m.id));
    const np=getPhotos('m'+m.id).length;const ds=datesSummary(m);
    const head=`<div class="mhtop"><span class="mtitle">${m.title||'Momento'}</span><button class="mdel medit" data-edit="${m.id}">✏️</button><button class="mdel" data-id="${m.id}">🗑️</button><span class="chev">▼</span></div><div class="mhmeta">${placesSummary(m)}${ds?`<span class="mtag">${ds}</span>`:''}${m.author?`<span class="mtag">${authorChip(m.author)}</span>`:''}${np?`<span class="mtag">📷 ${np}</span>`:''}</div>`;
    let body;
    if(editing){body=inlineEditorHTML(m);}
    else{const pills=momentPlaces(m).length>1?placesPills(m):'';body=`${pills?`<div class="mhmeta" style="margin-top:0">${pills}</div>`:''}${m.note?`<div class="mnote">${m.note}</div>`:''}${photoViewBlock('m'+m.id)}`;}
    return `<div class="moment${editing?' open editing':''}"><div class="mhead" data-mtoggle>${head}</div><div class="mbody">${body}</div></div>`;
  }).join('');
  list.querySelectorAll('[data-mtoggle]').forEach(h=>{h.addEventListener('click',e=>{if(e.target.closest('.mdel'))return;if(h.closest('.moment').classList.contains('editing'))return;h.closest('.moment').classList.toggle('open');});});
  list.querySelectorAll('[data-edit]').forEach(b=>{b.addEventListener('click',e=>{e.stopPropagation();startEdit(b.dataset.edit);});});
  list.querySelectorAll('.mdel[data-id]').forEach(b=>{b.addEventListener('click',()=>{const id=b.dataset.id;appConfirm('Apagar este momento?',()=>{store.del('ph_m'+id);setMoments(getMoments().filter(x=>String(x.id)!==String(id)));editingId=null;reRenderAll();});});});
  bindInlineEditors(list);
  bindCards(list);
}
function bindInlineEditors(root){
  const ed=root.querySelector('.ineditor');if(!ed)return;
  ed.querySelector('.ie-title').addEventListener('input',e=>editState.title=e.target.value);
  ed.querySelector('.ie-note').addEventListener('input',e=>editState.note=e.target.value);
  const pin=ed.querySelector('.ie-place');
  function addIE(v){v=(v||'').trim();if(v&&!editState.places.includes(v))editState.places.push(v);renderMoments();}
  ed.querySelector('.ie-addplace').addEventListener('click',()=>addIE(pin.value));
  pin.addEventListener('keydown',e=>{if(e.key==='Enter'){e.preventDefault();addIE(pin.value);}});
  ed.querySelector('.ie-listplace').addEventListener('click',()=>{window.placePickCb=(n)=>{if(!editState.places.includes(n))editState.places.push(n);renderMoments();};resetPlaceList();placeModal.classList.add('open');});
  ed.querySelectorAll('[data-iep]').forEach(b=>b.addEventListener('click',()=>{editState.places.splice(b.dataset.iep,1);renderMoments();}));
  ed.querySelector('.ie-daysbtn').addEventListener('click',()=>openDayPicker(editState.dates,()=>renderMoments()));
  ed.querySelector('.ie-addphoto').addEventListener('change',async e=>{const files=[...e.target.files];if(!files.length)return;const key=e.target.dataset.key;const arr=getPhotos(key);let ok=0;for(const file of files){try{const data=await processImage(file);arr.push({src:data,author:userName(),ts:nowTs()});ok++;}catch(err){}}setPhotos(key,arr);renderMoments();if(ok)toast(ok>1?(ok+' fotos adicionadas 📷'):'Foto adicionada 📷');});
  ed.querySelectorAll('.ie-rmphoto').forEach(b=>b.addEventListener('click',e=>{e.stopPropagation();const key=b.dataset.key;const arr=getPhotos(key);arr.splice(parseInt(b.dataset.idx),1);setPhotos(key,arr);renderMoments();}));
  ed.querySelector('.ie-save').addEventListener('click',()=>{const moments=getMoments();const m=moments.find(x=>String(x.id)===String(editingId));if(m){m.title=editState.title.trim();m.note=editState.note.trim();m.places=editState.places.slice();m.dates=[...editState.dates].sort();m.place=m.places[0]||'';m.date=m.dates[0]||'';setMoments(moments);}editingId=null;reRenderAll();toast('Alterações salvas ✨');});
  ed.querySelector('.ie-cancel').addEventListener('click',()=>{editingId=null;renderMoments();});
}
let editingId=null;
function clearForm(){formPhotos=[];renderFormPhotos();formPlaces=[];renderFormPlaces();formDaysSet=new Set();renderFormDays();$on('mTitle').value='';$on('mPlace').value='';$on('mNote').value='';editingId=null;$on('addMoment').textContent='💛 Salvar momento';}
function startEdit(id){const m=getMoments().find(x=>String(x.id)===String(id));if(!m)return;editingId=m.id;editState={title:m.title||'',note:m.note||'',places:momentPlaces(m).slice(),dates:new Set(momentDates(m))};renderMoments();}
$on('addPlaceBtn').addEventListener('click',()=>{addFormPlace($on('mPlace').value);$on('mPlace').value='';});
$on('mPlace').addEventListener('keydown',e=>{if(e.key==='Enter'){e.preventDefault();addFormPlace($on('mPlace').value);$on('mPlace').value='';}});
$on('addMoment').addEventListener('click',()=>{
  const title=$on('mTitle').value.trim();
  const note=$on('mNote').value.trim();
  const pend=$on('mPlace').value.trim();if(pend){addFormPlace(pend);$on('mPlace').value='';}
  const dates=[...formDaysSet].sort();
  if(!dates.length){appNotice('Escolha pelo menos um dia da viagem para este momento.');return;}
  const places=formPlaces.slice();
  const id=nowTs();const moments=getMoments();moments.push({id,title,note,places,dates,place:places[0]||'',date:dates[0]||'',author:userName(),ts:id});setMoments(moments);
  if(formPhotos.length){setPhotos('m'+id,formPhotos.slice());}
  clearForm();$on('mform').classList.remove('open');reRenderAll();toast('Momento salvo 💛');
});

function momentMatches(m,q){
  if(!q)return true;q=q.toLowerCase();
  if(momentPlaces(m).some(p=>(p||'').toLowerCase().includes(q)))return true;
  if(momentDates(m).some(d=>(d||'').includes(q)))return true;
  if((m.title||'').toLowerCase().includes(q))return true;
  if((m.place||'').toLowerCase().includes(q))return true;
  if((m.note||'').toLowerCase().includes(q))return true;
  if((m.author||'').toLowerCase().includes(q))return true;
  if((m.date||'').includes(q))return true;
  const photos=getPhotos('m'+m.id);
  return photos.some(p=>(p.caption||'').toLowerCase().includes(q));
}
function renderAlbum(){
  const el=$on('albumFeed');
  const q=($on('albumSearch')||{}).value||'';
  let moments=getMoments().slice().sort((a,b)=>momentKey(a)-momentKey(b));
  moments=moments.filter(m=>momentMatches(m,q)&&(!albumDaysSet.size||momentDates(m).some(d=>albumDaysSet.has(d)))&&(!albumCity||momentPlaces(m).some(p=>placeClass(p)===albumCity)));
  if(!moments.length){el.innerHTML='<div class="empty">'+((q||albumDaysSet.size||albumCity)?'Nada encontrado para esse filtro.':'Ainda não há momentos. Crie momentos no Diário e eles aparecem aqui em linha do tempo.')+'</div>';updateFloatDate();return;}
  el.innerHTML='<div class="timeline">'+moments.map(m=>{
    const rows=photoRowsAlbum('m'+m.id);
    const dts=momentDates(m);const floatd=dts.length?dmy(dts[0]):'';
    const dshort=datesSummary(m).replace('📅 ','');
    return `<div class="tlitem" data-date="${floatd}"><div class="tldot"></div>${dshort?`<div class="tldatedot">${dshort}</div>`:''}<div class="tlcard"><div class="tltitle">${m.title||'Momento'}${m.author?` <span class="tlauthor">${authorChip(m.author)}</span>`:''}</div>${placesPills(m)?`<div class="mhmeta tlplaces">${placesPills(m)}</div>`:''}${m.note?`<div class="photocap">${escHtml(m.note)}</div>`:''}${rows?`<div class="photorows">${rows}</div>`:''}</div></div>`;
  }).join('')+'</div>';
  bindCards(el);updateFloatDate();
}
function updateFloatDate(){
  const fl=$on('albumDateFloat');if(!fl)return;
  if(!$on('album').classList.contains('active')){fl.style.display='none';return;}
  const items=document.querySelectorAll('#albumFeed .tlitem');let cur='';
  items.forEach(it=>{if(it.getBoundingClientRect().top<150)cur=it.dataset.date||cur;});
  if(cur){fl.textContent='📅 '+cur;fl.style.display='block';}else{fl.style.display='none';}
}
function updateCounts(){$on('cMoments').textContent=getMoments().length;let p=0;store.keys().forEach(k=>{if(k.indexOf('ph_')===0){try{p+=JSON.parse(store.get(k)).length;}catch(e){}}});$on('cPhotos').textContent=p;}

/* PLACE PICKER */
const placeModal=$on('placeModal');
function buildPlaceList(){
  const disneyAttr=DIA1.concat(DIA2).filter(it=>!it.special).map(it=>it.n);
  const groups=[['Paris',PARIS_PLACES],['Disney',[...new Set(DISNEY_PLACES.concat(disneyAttr))]],['Bruxelas',BRUXELAS_PLACES],['Bruges',BRUGES_PLACES],['Amsterdam',AMSTERDAM_PLACES],['Geral',GERAL_PLACES]];
  $on('placeList').innerHTML=groups.map(([g,arr])=>`<div class="plgroup">${g}</div>`+arr.map(n=>`<button data-place="${n}">${n}</button>`).join('')).join('');
  $on('placeList').querySelectorAll('[data-place]').forEach(b=>b.addEventListener('click',()=>{const n=b.dataset.place;if(window.placePickCb){window.placePickCb(n);}else{addFormPlace(n);}b.classList.add('picked');b.textContent='✓ '+n;toast('Local adicionado 📍');}));
  const allNames=[];groups.forEach(([g,arr])=>arr.forEach(n=>allNames.push(n)));
  KNOWN_PLACES=new Set(allNames);
  $on('placeSuggestions').innerHTML=[...new Set(allNames)].map(n=>`<option value="${n}">`).join('');
}

/* DATA collect + merge (only adds) */
function collectData(){const data={checks:{},photos:{},moments:getMoments(),profiles:{}};store.keys().forEach(k=>{if(k.indexOf('ph_')===0){try{data.photos[k]=JSON.parse(store.get(k));}catch(e){}}else if((k.indexOf('d1_')===0||k.indexOf('d2_')===0)&&store.get(k)==='1'){data.checks[k]=1;}else if(k.indexOf('profile_')===0){data.profiles[k]=store.get(k);}});return data;}
function photoSig(p){const s=typeof p==='string'?p:p.src;return (p.author||'')+'|'+(p.ts||'')+'|'+s.length+'|'+s.slice(0,40);}
function mergeData(data){
  if(!data)return;
  if(data.checks){Object.keys(data.checks).forEach(k=>store.set(k,'1'));}
  if(data.profiles){Object.keys(data.profiles).forEach(k=>{if(!store.get(k))store.set(k,data.profiles[k]);});}
  if(data.photos){Object.keys(data.photos).forEach(k=>{let existing=[];try{existing=JSON.parse(store.get(k)||'[]');}catch(e){}const seen={};const merged=[];existing.concat(data.photos[k]).forEach(p=>{const sig=photoSig(p);if(!seen[sig]){seen[sig]=1;merged.push(typeof p==='string'?{src:p,author:'',ts:0}:p);}});store.set(k,JSON.stringify(merged));});}
  if(data.moments){const map={};getMoments().forEach(m=>map[m.id]=m);data.moments.forEach(m=>{if(!map[m.id])map[m.id]=m;});setMoments(Object.values(map).sort((a,b)=>momentKey(a)-momentKey(b)));}
}

/* MODALS */
const syncModal=$on('syncModal');
const gearModal=$on('gearModal');

const modal=$on('modal'),modalText=$on('modalText'),modalTitle=$on('modalTitle'),modalDesc=$on('modalDesc'),modalAction=$on('modalAction');
let modalMode='export';
function openTextModal(mode){
  syncModal.classList.remove('open');
  modalMode=mode;
  if(mode==='export'){modalTitle.textContent='⬆️ Meu código';modalDesc.textContent='Este código tem suas fotos, momentos e perfil. Toque em Copiar e envie para o Edson, que vai juntar tudo.';modalText.value=JSON.stringify(collectData());modalText.readOnly=true;modalAction.textContent='📋 Copiar';}
  else if(mode==='import'){modalTitle.textContent='⬇️ Juntar um código';modalDesc.textContent='Cole aqui o código que alguém da família enviou e toque em Juntar. Ele soma tudo, sem apagar o que você já tem.';modalText.value='';modalText.readOnly=false;modalAction.textContent='♻️ Juntar';}
  modal.classList.add('open');
}
function exportFile(){
  syncModal.classList.remove('open');
  try{
    const data=JSON.stringify(collectData());
    const blob=new Blob([data],{type:'text/plain'});
    const url=URL.createObjectURL(blob);
    const nm=(userName()||'familia').replace(/[^a-z0-9]/gi,'_').toLowerCase();
    const d=new Date();const stamp=d.getFullYear()+String(d.getMonth()+1).padStart(2,'0')+String(d.getDate()).padStart(2,'0');
    const a=document.createElement('a');a.href=url;a.download='memorias_'+nm+'_'+stamp+'.txt';document.body.appendChild(a);a.click();document.body.removeChild(a);
    setTimeout(()=>URL.revokeObjectURL(url),5000);
    toast('Arquivo de memórias baixado 💾');
    appNotice('Pronto! Baixei um arquivo com suas memórias. Envie ele para outro celular (WhatsApp, e-mail...) e lá use Importar para abrir o arquivo e carregar tudo.');
  }catch(e){appNotice('Não consegui gerar o arquivo neste navegador.');}
}
$on('optExport').addEventListener('click',exportFile);
$on('optImport').addEventListener('click',()=>{syncModal.classList.remove('open');$on('importFile').click();});
$on('importFile').addEventListener('change',e=>{
  const file=e.target.files[0];if(!file)return;
  const reader=new FileReader();
  reader.onload=()=>{
    let data;try{data=JSON.parse(reader.result);}catch(err){appNotice('O arquivo não parece válido. Use o arquivo .txt exportado pelo app.');return;}
    appConfirm('Juntar as memórias deste arquivo às suas? Nada será apagado, tudo será somado.',()=>{mergeData(data);refreshAvatars();refreshWhoChip();reRenderAll();toast('Memórias do arquivo carregadas! 💛');});
  };
  reader.onerror=()=>appNotice('Não consegui ler o arquivo.');
  reader.readAsText(file);
  e.target.value='';
});
modalAction.addEventListener('click',()=>{
  if(modalMode==='export'||modalMode==='fullhtml'){modalText.select();try{if(navigator.clipboard){navigator.clipboard.writeText(modalText.value);}else{document.execCommand('copy');}modalAction.textContent='✅ Copiado!';setTimeout(()=>modalAction.textContent='📋 Copiar',1800);}catch(e){alert('Selecione o texto e copie manualmente.');}}
  else if(modalMode==='import'){let data;try{data=JSON.parse(modalText.value.trim());}catch(e){alert('O código não parece válido. Confira se colou ele inteiro.');return;}appConfirm('Juntar este código às suas memórias? Nada será apagado, tudo será somado.',()=>{mergeData(data);modal.classList.remove('open');refreshAvatars();refreshWhoChip();reRenderAll();toast('Memórias juntadas! 💛');});}
});

async function copyFullHtml(){
  gearModal.classList.remove('open');
  let html;
  try{const res=await fetch(window.location.href,{cache:'no-store'});html=await res.text();}catch(e){appNotice('Para gerar o site completo, abra pelo link do GitHub Pages (https), não pelo arquivo local.');return;}
  const json=JSON.stringify(collectData()).replace(/</g,'\\u003c');
  const replacement='/*__DATA_START__*/\nwindow.EMBEDDED_DATA = '+json+';\n/*__DATA_END__*/';
  const re=/\/\*__DATA_START__\*\/[\s\S]*?\/\*__DATA_END__\*\//;
  if(!re.test(html)){appNotice('Não encontrei o marcador no arquivo. Verifique se está usando o index.html gerado.');return;}
  html=html.replace(re,replacement);
  try{
    const blob=new Blob([html],{type:'text/html'});
    const url=URL.createObjectURL(blob);
    const a=document.createElement('a');a.href=url;a.download='index.html';document.body.appendChild(a);a.click();document.body.removeChild(a);
    setTi
