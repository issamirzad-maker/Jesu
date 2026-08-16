# Jesu<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<title>بی‌وفا | نمای افتتاحیه</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Vazirmatn:wght@200;300;400;700;900&display=swap');

  :root{
    --bg:#070707;
    --crimson:#7a1f2b;
    --crimson-bright:#b23a3a;
    --gold:#a68a5b;
    --fog:#8c8c8c;
  }

  *{margin:0;padding:0;box-sizing:border-box;}

  html,body{
    width:100%;height:100%;
    background:var(--bg);
    overflow:hidden;
    font-family:'Vazirmatn',sans-serif;
  }

  .stage{
    position:relative;
    width:100vw;height:100vh;
    display:flex;align-items:center;justify-content:center;
    background:radial-gradient(ellipse at center, #141414 0%, #050505 70%, #000 100%);
  }

  .bar{
    position:absolute;left:0;width:100%;height:9vh;
    background:#000;
    z-index:10;
  }
  .bar.top{top:0; transform:translateY(-100%); animation: dropBar 1.4s 0.2s ease forwards;}
  .bar.bottom{bottom:0; transform:translateY(100%); animation: dropBarB 1.4s 0.2s ease forwards;}
  @keyframes dropBar{to{transform:translateY(0);}}
  @keyframes dropBarB{to{transform:translateY(0);}}

  .grain{
    position:absolute;inset:0;
    z-index:5;
    opacity:0.08;
    pointer-events:none;
    background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='120' height='120'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='2' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
    animation:grainMove 0.4s steps(4) infinite;
  }
  @keyframes grainMove{
    0%{transform:translate(0,0);} 25%{transform:translate(-2%,1%);}
    50%{transform:translate(1%,-2%);} 75%{transform:translate(-1%,2%);}
    100%{transform:translate(0,0);}
  }

  .haze{
    position:absolute;inset:0;
    background:radial-gradient

    
