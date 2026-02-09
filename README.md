<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8">
  <title>แบบประเมินความเครียด</title>

  <!-- ===== CSS ===== -->
  <style>
    * {
      box-sizing: border-box;
      font-family: 'Segoe UI', sans-serif;
    }

    body {
      margin: 0;
      min-height: 100vh;
      background: linear-gradient(120deg, #fff1eb, #cdeffd);
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .container {
      width: 100%;
      display: flex;
      justify-content: center;
    }

    .card {
      background: #fff;
      width: 800px;
      padding: 32px;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.1);
      text-align: left;
    }

    h2 {
      text-align: center;
    }

    .subtitle {
      color: #666;
      font-size: 14px;
      margin-bottom: 20px;
      text-align: center;
    }

    .question {
      margin-bottom: 24px;
    }

    .question p {
      font-weight: 500;
    }

    .question label {
      margin-right: 16px;
      font-size: 14px;
    }

    .btn {
      width: 100%;
      padding: 14px;
      border-radius: 12px;
      border: none;
      margin-top: 12px;
      font-size: 16px;
      cursor: pointer;
      background: #ffd8c2;
    }

    .btn.primary {
      background: #ff9f68;
      color: white;
    }

    .btn:hover {
      opacity: 0.9;
    }

    #result {
      margin-top: 20px;
      font-weight: bold;
      text-align: center;
    }
  </style>
</head>

<body>
  <div class="container">
    <div class="card">
      <h2>แบบประเมินความเครียด</h2>
      <p class="subtitle">
        ในระยะเวลา 2 เดือนที่ผ่านมา โปรดเลือกระดับที่ตรงกับคุณมากที่สุด
      </p>

      <form id="stressForm">

        <!-- ข้อ 1 - 20 -->
        <!-- (โครงสร้างเหมือนกันทุกข้อ) -->

        <div class="question">
          <p>1. นอนไม่หลับเพราะคิดมากหรือกังวลใจ</p>
          <label><input type="radio" name="q1" value="0"> ไม่เคยเลย</label>
          <label><input type="radio" name="q1" value="1"> เป็นครั้งคราว</label>
          <label><input type="radio" name="q1" value="2"> เป็นบ่อย</label>
          <label><input type="radio" name="q1" value="3"> เป็นประจำ</label>
        </div>

        <div class="question">
          <p>2. รู้สึกหงุดหงิด รำคาญใจ</p>
          <label><input type="radio" name="q2" value="0"> ไม่เคยเลย</label>
          <label><input type="radio" name="q2" value="1"> เป็นครั้งคราว</label>
          <label><input type="radio" name="q2" value="2"> เป็นบ่อย</label>
          <label><input type="radio" name="q2" value="3"> เป็นประจำ</label>
        </div>

        <div class="question">
    <p>3. ทำอะไรไม่ได้เลยเพราะประสาทตึงเครียด</p>
    <label><input type="radio" name="q3" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q3" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q3" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q3" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>4. มีความวุ่นวายใจ</p>
    <label><input type="radio" name="q4" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q4" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q4" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q4" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>5. ไม่อยากพบปะผู้คน</p>
    <label><input type="radio" name="q5" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q5" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q5" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q5" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>6. ปวดหัวข้างเดียว หรือปวดบริเวณขมับทั้ง 2 ข้าง</p>
    <label><input type="radio" name="q6" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q6" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q6" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q6" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>7. รู้สึกไม่มีความสุขและเศร้าหมอง</p>
    <label><input type="radio" name="q7" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q7" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q7" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q7" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>8. รู้สึกหมดหวังในชีวิต</p>
    <label><input type="radio" name="q8" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q8" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q8" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q8" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>9. รู้สึกชีวิตตนเองไม่มีคุณค่า</p>
    <label><input type="radio" name="q9" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q9" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q9" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q9" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>10. กระวนกระวายอยู่ตลอดเวลา</p>
    <label><input type="radio" name="q10" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q10" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q10" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q10" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>11. รู้สึกว่าตนเองไม่มีสมาธิ</p>
    <label><input type="radio" name="q11" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q11" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q11" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q11" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>12. รู้สึกเพลียจนไม่มีแรงจะทำอะไร</p>
    <label><input type="radio" name="q12" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q12" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q12" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q12" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>13. รู้สึกเหนื่อยหน่ายไม่อยากทำอะไร</p>
    <label><input type="radio" name="q13" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q13" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q13" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q13" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>14. มีอาการหัวใจเต้นแรง</p>
    <label><input type="radio" name="q14" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q14" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q14" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q14" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>15. เสียงสั่น ปากสั่น หรือมือสั่นเวลาไม่พอใจ</p>
    <label><input type="radio" name="q15" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q15" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q15" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q15" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>16. รู้สึกกลัวผิดพลาดในการทำสิ่งต่าง ๆ</p>
    <label><input type="radio" name="q16" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q16" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q16" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q16" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>17. ปวดหรือเกร็งกล้ามเนื้อบริเวณท้ายทอย หลัง หรือไหล่</p>
    <label><input type="radio" name="q17" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q17" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q17" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q17" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>18. ตื่นเต้นง่ายกับเหตุการณ์ที่ไม่คุ้นเคย</p>
    <label><input type="radio" name="q18" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q18" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q18" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q18" value="3"> เป็นประจำ</label>
  </div>

  <div class="question">
    <p>19. มึนงงหรือเวียนศีรษะ</p>
    <label><input type="radio" name="q19" value="0"> ไม่เคยเลย</label>
    <label><input type="radio" name="q19" value="1"> เป็นครั้งคราว</label>
    <label><input type="radio" name="q19" value="2"> เป็นบ่อย</label>
    <label><input type="radio" name="q19" value="3"> เป็นประจำ</label>
  </div>

        <!-- ... (ข้อ 3–19 เหมือนเดิมทุกประการ) ... -->

        <div class="question">
          <p>20. ความสุขทางเพศลดลง</p>
          <label><input type="radio" name="q20" value="0"> ไม่เคยเลย</label>
          <label><input type="radio" name="q20" value="1"> เป็นครั้งคราว</label>
          <label><input type="radio" name="q20" value="2"> เป็นบ่อย</label>
          <label><input type="radio" name="q20" value="3"> เป็นประจำ</label>
        </div>

        <button type="button" class="btn primary" onclick="calculateScore()">
          ดูผลการประเมิน
        </button>
      </form>

      <p id="result"></p>
    </div>
  </div>

  <!-- ===== JavaScript ===== -->
  <script>
    function calculateScore() {
      let total = 0;

      for (let i = 1; i <= 20; i++) {
        const answer = document.querySelector(`input[name="q${i}"]:checked`);
        if (!answer) {
          alert("กรุณาตอบให้ครบทุกข้อ");
          return;
        }
        total += parseInt(answer.value);
      }

      let resultText = "";

      if (total <= 23) {
        resultText = "ความเครียดอยู่ในระดับต่ำ 😊";
      } else if (total <= 41) {
        resultText = "ความเครียดระดับปานกลาง ควรดูแลตัวเองให้มากขึ้น 💛";
      } else {
        resultText = "ความเครียดอยู่ในระดับสูง แนะนำให้ปรึกษาผู้เชี่ยวชาญ ☎️ 1323";
      }

      document.getElementById("result").innerText =
        `คะแนนรวม: ${total} คะแนน\n${resultText}`;
    }
  </script>
</body>
</html>
