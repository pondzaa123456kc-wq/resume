  
<!DOCTYPE html>  
<html lang="th">  
<head>  
  <meta charset="UTF-8">  
  <meta name="viewport" content="width=device-width, initial-scale=1.0">  
  <title>Resume | อภินพ ส่งเสริม</title>  
  
  <style>  
    * {  
      margin: 0;  
      padding: 0;  
      box-sizing: border-box;  
    }  
  
    html {  
      scroll-behavior: smooth;  
    }  
  
    body {  
      font-family: Tahoma, Arial, sans-serif;  
      background: #f4f6fb;  
      color: #20243a;  
      line-height: 1.7;  
    }  
  
    .container {  
      width: 90%;  
      max-width: 1050px;  
      margin: auto;  
    }  
  
    header {  
      padding: 22px 0;  
      background: white;  
      border-bottom: 1px solid #e5e7f0;  
    }  
  
    nav {  
      display: flex;  
      justify-content: space-between;  
      align-items: center;  
      flex-wrap: wrap;  
      gap: 12px;  
    }  
  
    .logo {  
      font-size: 22px;  
      font-weight: bold;  
      color: #5b5ce2;  
    }  
  
    nav a {  
      text-decoration: none;  
      color: #555b70;  
      margin-left: 16px;  
    }  
  
    nav a:hover {  
      color: #5b5ce2;  
    }  
  
    .hero {  
      display: grid;  
      grid-template-columns: 1.5fr 1fr;  
      gap: 35px;  
      align-items: center;  
      padding: 75px 0;  
    }  
  
    .badge {  
      display: inline-block;  
      background: #e8e9ff;  
      color: #4d4ec7;  
      padding: 7px 15px;  
      border-radius: 30px;  
      font-size: 13px;  
      margin-bottom: 18px;  
    }  
  
    h1 {  
      font-size: clamp(32px, 5vw, 50px);  
      line-height: 1.3;  
      margin-bottom: 18px;  
    }  
  
    .highlight {  
      color: #5b5ce2;  
    }  
  
    .intro {  
      color: #687087;  
      margin-bottom: 25px;  
    }  
  
    .button {  
      display: inline-block;  
      padding: 11px 20px;  
      margin: 4px 5px 4px 0;  
      border-radius: 10px;  
      text-decoration: none;  
      font-weight: bold;  
      background: #5b5ce2;  
      color: white;  
    }  
  
    .button:hover {  
      background: #4142bd;  
    }  
  
    .button.light {  
      background: white;  
      color: #5b5ce2;  
      border: 1px solid #ddd;  
    }  
  
    .profile {  
      background: white;  
      padding: 30px;  
      border-radius: 25px;  
      box-shadow: 0 12px 35px #20243a12;  
      text-align: center;  
    }  
  
    .avatar {  
      width: 100px;  
      height: 100px;  
      display: grid;  
      place-items: center;  
      margin: 0 auto 20px;  
      background: linear-gradient(135deg, #8586ff, #4142bd);  
      color: white;  
      border-radius: 25px;  
      font-size: 34px;  
      font-weight: bold;  
    }  
  
    .profile p {  
      color: #687087;  
    }  
  
    .tags {  
      display: flex;  
      justify-content: center;  
      flex-wrap: wrap;  
      gap: 8px;  
      margin-top: 18px;  
    }  
  
    .tag {  
      background: #f0f1f8;  
      padding: 6px 10px;  
      border-radius: 8px;  
      font-size: 12px;  
    }  
  
    section {  
      padding: 30px 0;  
    }  
  
    .section-title {  
      margin-bottom: 22px;  
    }  
  
    .section-title small {  
      color: #5b5ce2;  
      font-weight: bold;  
      letter-spacing: 2px;  
    }  
  
    .section-title h2 {  
      font-size: 30px;  
      margin-top: 5px;  
    }  
  
    .section-title p {  
      color: #687087;  
      margin-top: 5px;  
    }  
  
    .grid {  
      display: grid;  
      grid-template-columns: repeat(3, 1fr);  
      gap: 18px;  
    }  
  
    .card {  
      background: white;  
      padding: 25px;  
      border-radius: 18px;  
      border: 1px solid #e8eaf2;  
    }  
  
    .card h3 {  
      margin-bottom: 10px;  
    }  
  
    .card p {  
      color: #687087;  
      font-size: 14px;  
    }  
  
    .info {  
      display: grid;  
      grid-template-columns: 1fr 1fr;  
      gap: 18px;  
    }  
  
    .info-row {  
      padding: 12px 0;  
      border-bottom: 1px solid #e8eaf2;  
    }  
  
    .info-row strong {  
      display: block;  
      margin-bottom: 3px;  
    }  
  
    .info-row span {  
      color: #687087;  
    }  
  
    .icon {  
      font-size: 28px;  
      margin-bottom: 12px;  
    }  
  
    .project {  
      background: #eeeeff;  
      border: 1px dashed #b9bbf5;  
      padding: 25px;  
      border-radius: 12px;  
      margin-bottom: 15px;  
      text-align: center;  
      font-size: 30px;  
    }  
  
    .contact {  
      background: linear-gradient(120deg, #27295f, #6263e8);  
      color: white;  
      padding: 35px;  
      border-radius: 22px;  
      margin: 35px 0 55px;  
    }  
  
    .contact p {  
      color: #e2e3ff;  
      margin: 8px 0 18px;  
    }  
  
    .contact a {  
      color: white;  
    }  
  
    footer {  
      padding: 25px 0;  
      text-align: center;  
      color: #687087;  
      border-top: 1px solid #e5e7f0;  
      font-size: 13px;  
    }  
  
    @media (max-width: 700px) {  
      .hero,  
      .info {  
        grid-template-columns: 1fr;  
      }  
  
      .hero {  
        padding: 45px 0;  
      }  
  
      .grid {  
        grid-template-columns: 1fr;  
      }  
  
      nav {  
        flex-direction: column;  
        align-items: flex-start;  
      }  
  
      nav a {  
        margin-left: 0;  
        margin-right: 12px;  
      }  
  
      .section-title h2 {  
        font-size: 25px;  
      }  
  
      .contact {  
        padding: 25px;  
      }  
    }  
  </style>  
</head>  
  
<body>  
  
  <header>  
    <div class="container">  
      <nav>  
        <div class="logo">MY RESUME</div>  
        <div>  
          <a href="#about">เกี่ยวกับฉัน</a>  
          <a href="#skills">ทักษะ</a>  
          <a href="#projects">ผลงาน</a>  
          <a href="#contact">ติดต่อ</a>  
        </div>  
      </nav>  
    </div>  
  </header>  
  
  <main class="container">  
  
    <!-- ส่วนแนะนำตัว -->  
    <section class="hero">  
      <div>  
        <span class="badge">COMMUNICATION ARTS STUDENT</span>  
  
        <h1>  
          สวัสดีครับ<br>  
          ผมชื่อ <span class="highlight">อภินพ ส่งเสริม</span>  
        </h1>  
  
        <p class="intro">  
          นักศึกษาสาขานิเทศศาสตร์ มหาวิทยาลัยหอการค้าไทย  
          สนใจการสร้างสรรค์สื่อ การตัดต่อวิดีโอ การถ่ายภาพ  
          และการนำเทคโนโลยี AI มาประยุกต์ใช้ในการทำงาน  
        </p>  
  
        <a href="#projects" class="button">ดูผลงานของฉัน</a>  
        <a href="#contact" class="button light">ติดต่อฉัน</a>  
      </div>  
  
      <div class="profile">  
        <div class="avatar">อส</div>  
        <h2>อภินพ ส่งเสริม</h2>  
        <p>นักศึกษานิเทศศาสตร์</p>  
  
        <div class="tags">  
          <span class="tag">Video Editing</span>  
          <span class="tag">Photography</span>  
          <span class="tag">AI Tools</span>  
          <span class="tag">Media Production</span>  
        </div>  
      </div>  
    </section>  
  
    <!-- เกี่ยวกับฉัน -->  
    <section id="about">  
      <div class="section-title">  
        <small>ABOUT ME</small>  
        <h2>เกี่ยวกับฉัน</h2>  
        <p>ประวัติส่วนตัวและข้อมูลการศึกษา</p>  
      </div>  
  
      <div class="info">  
        <div class="card">  
          <h3>ข้อมูลส่วนตัว</h3>  
  
          <div class="info-row">  
            <strong>ชื่อ-นามสกุล</strong>  
            <span>อภินพ ส่งเสริม</span>  
          </div>  
  
          <div class="info-row">  
            <strong>สาขาวิชา</strong>  
            <span>นิเทศศาสตร์</span>  
          </div>  
  
          <div class="info-row">  
            <strong>มหาวิทยาลัย</strong>  
            <span>มหาวิทยาลัยหอการค้าไทย</span>  
          </div>  
  
          <div class="info-row">  
            <strong>สถานะ</strong>  
            <span>นักศึกษา</span>  
          </div>  
        </div>  
  
        <div class="card">  
          <h3>แนะนำตัว</h3>  
          <p>  
            ผมเป็นนักศึกษานิเทศศาสตร์ที่สนใจการผลิตสื่อ  
            และการสื่อสารผ่านภาพและวิดีโอ มีความสนใจด้านการตัดต่อ  
            การถ่ายภาพ และการใช้ AI เพื่อช่วยสร้างสรรค์ไอเดีย  
            พร้อมเรียนรู้ทักษะใหม่ ๆ และพัฒนาตัวเองอย่างต่อเนื่อง  
          </p>  
        </div>  
      </div>  
    </section>  
  
    <!-- ทักษะ -->  
    <section id="skills">  
      <div class="section-title">  
        <small>MY SKILLS</small>  
        <h2>ทักษะของฉัน</h2>  
        <p>ทักษะที่สนใจและนำไปพัฒนาต่อยอด</p>  
      </div>  
  
      <div class="grid">  
        <div class="card">  
          <div class="icon">🎬</div>  
          <h3>ตัดต่อวิดีโอ</h3>  
          <p>  
            เรียบเรียงภาพและเสียง เลือกจังหวะการตัดต่อ  
            เพื่อเล่าเรื่องให้น่าสนใจและเข้าใจง่าย  
          </p>  
        </div>  
  
        <div class="card">  
          <div class="icon">📷</div>  
          <h3>ถ่ายภาพ</h3>  
          <p>  
            สนใจการจัดองค์ประกอบภาพ มุมกล้อง แสง  
            และการใช้ภาพเพื่อถ่ายทอดเรื่องราว  
          </p>  
        </div>  
  
        <div class="card">  
          <div class="icon">✨</div>  
          <h3>การใช้ AI</h3>  
          <p>  
            ใช้เครื่องมือ AI เพื่อช่วยระดมความคิด  
            วางแผน และสนับสนุนการสร้างสรรค์ผลงานสื่อ  
          </p>  
        </div>  
      </div>  
    </section>  
  
    <!-- ประสบการณ์และผลงาน -->  
    <section id="projects">  
      <div class="section-title">  
        <small>EXPERIENCE & PROJECTS</small>  
        <h2>ประสบการณ์และผลงาน</h2>  
        <p>  
          นักศึกษาที่กำลังพัฒนาทักษะด้านนิเทศศาสตร์  
          สามารถเพิ่มผลงานจากการเรียนได้ในส่วนนี้  
        </p>  
      </div>  
  
      <div class="grid">  
        <div class="card">  
          <div class="project">🎞️</div>  
          <h3>ผลงานตัดต่อวิดีโอ</h3>  
          <p>  
            เพิ่มรายละเอียดคลิปวิดีโอ หนังสั้น  
            หรือผลงานตัดต่อที่เคยทำ  
          </p>  
        </div>  
  
        <div class="card">  
          <div class="project">📸</div>  
          <h3>ผลงานถ่ายภาพ</h3>  
          <p>  
            เพิ่มภาพถ่ายที่สนใจ พร้อมอธิบายแนวคิด  
            และเทคนิคที่ใช้ในการถ่ายภาพ  
          </p>  
        </div>  
  
        <div class="card">  
          <div class="project">💡</div>  
          <h3>โปรเจกต์สร้างสรรค์</h3>  
          <p>  
            เพิ่มงานกลุ่ม งานในชั้นเรียน  
            หรือโปรเจกต์ที่ใช้ AI ช่วยสร้างสรรค์สื่อ  
          </p>  
        </div>  
      </div>  
    </section>  
  
    <!-- ติดต่อ -->  
    <section id="contact">  
      <div class="contact">  
        <h2>ติดต่อฉัน</h2>  
        <p>  
          ขอบคุณที่เข้ามาเยี่ยมชม Resume ของผม  
          สามารถติดต่อสอบถามเพิ่มเติมได้ที่  
        </p>  
  
        <p>  
          โทรศัพท์:  
          <a href="tel:0958602375">095-860-2375</a>  
        </p>  
  
        <a href="tel:0958602375" class="button light">  
          โทรติดต่อ  
        </a>  
      </div>  
    </section>  
  
  </main>  
  
  <footer>  
    <div class="container">  
      © 2026 อภินพ ส่งเสริม | Resume Portfolio  
    </div>  
  </footer>  
  
</body>  
</html>  
