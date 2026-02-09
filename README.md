# Valentine-2026
<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<title>Belle & Grace 💖</title>
<style>
body{
  margin:0;
  font-family: 'Arial', sans-serif;
  background: linear-gradient(135deg,#ff9a9e,#fad0c4);
  color:#fff;
  display:flex;
  justify-content:center;
  align-items:center;
  height:100vh;
  text-align:center;
}
.card{
  background:rgba(255,255,255,0.15);
  padding:30px;
  border-radius:20px;
  max-width:350px;
}
img{
  width:100%;
  border-radius:15px;
  margin-bottom:15px;
}
button{
  margin-top:15px;
  padding:12px 25px;
  border:none;
  border-radius:25px;
  background:#ff4d6d;
  color:#fff;
  font-size:1rem;
}
</style>
</head>
<body>

<div class="card">
  <div id="content"></div>
  <button onclick="nextScene()">ถัดไป 💕</button>
</div>

<script>
const scenes = [
  `<h2>Happy Valentine’s Day 💖</h2>
   <p>ของขวัญวาเลนไทน์ปีนี้สำหรับเบล<br>คือมีเกรซอยู่ข้างๆ</p>`,

  `<img src="photo1.jpg">
   <p>ทุกอย่างเริ่มจากวันธรรมดา<br>ที่ทำให้หัวใจไม่ธรรมดา</p>`,

  `<img src="photo2.jpg">
   <p>ไม่ว่าจะอยู่ที่ไหน<br>ถ้ามีเธออยู่ตรงนั้น…คือบ้าน</p>`,

  `<img src="photo3.jpg">
   <p>รอยยิ้มของเธอ<br>คือสิ่งที่เราอยากเห็นทุกวัน</p>`,

  `<img src="photo4.jpg">
   <p>บางวันอาจเหนื่อย<br>แต่จับมือเธอไว้ก็ไหว</p>`,

  `<img src="photo5.jpg">
   <p>ความสุขของเรา<br>อยู่ในเรื่องเล็กๆ แบบนี้</p>`,

  `<img src="photo6.jpg">
   <p>ขอบคุณที่อยู่ด้วยกัน<br>แม้วันที่ไม่น่ารัก</p>`,

  `<img src="photo7.jpg">
   <p>วันนี้เราอยากมีเธออยู่ตรงนี้</p>`,

  `<p>รักของเราอาจไม่สมบูรณ์แบบ<br>แต่ตั้งใจรักจริงๆ</p>`,

  `<h2>Happy Valentine’s Day 💖</h2>
   <p>รักเกรซนะ<br>จากเบล 🌷</p>`
];

let i = 0;
const content = document.getElementById("content");
content.innerHTML = scenes[i];

function nextScene(){
  i++;
  if(i < scenes.length){
    content.innerHTML = scenes[i];
  }
}
</script>

</body>
</html>
