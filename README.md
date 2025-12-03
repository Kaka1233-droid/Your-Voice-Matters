<html lang="th">
<head>
  <meta charset="UTF-8" />
  <title>พูดแทนใจ Your Voice Matters</title>

  <!-- Google Fonts: Prompt + Kanit -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Prompt:wght@300;400;500;600;700&family=Kanit:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>

  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            prompt: ['Prompt', 'system-ui', 'sans-serif'],
            kanit: ['Kanit', 'system-ui', 'sans-serif'],
          },
          colors: {
            softpink: '#FDE2FF',
            softpurple: '#E5D4FF',
            softblue: '#E0F2FF',
          },
        }
      }
    }
  </script>

  <style>
    body {
      font-family: 'Prompt', system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    }
    .font-kanit {
      font-family: 'Kanit', system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    }
  </style>
</head>
<body class="min-h-screen bg-gradient-to-br from-softblue via-softpink to-softpurple flex items-stretch justify-center">

  <div class="w-full max-w-6xl mx-auto p-4 sm:p-6 lg:p-8">
    <!-- กล่องหลัก -->
    <div class="bg-white/80 backdrop-blur-xl shadow-xl rounded-3xl p-4 sm:p-6 lg:p-8 border border-white/60">

      <!-- ส่วนหัว -->
      <header class="flex flex-col md:flex-row items-center md:items-start gap-4 md:gap-6 mb-6">
        <div class="flex-shrink-0">
          <img src="https://kkclassvip.com/wp-content/uploads/2025/05/heart-botnoi-voice.png"
               alt="Your Voice Matters Logo"
               class="w-24 h-auto mx-auto md:mx-0">
        </div>
        <div class="flex-1 text-center md:text-left">
          <h1 class="text-2xl sm:text-3xl lg:text-4xl font-semibold font-kanit text-purple-700 flex items-center justify-center md:justify-start gap-2">
            🗣️ พูดแทนใจ – Your Voice Matters
          </h1>
          <p class="mt-1 text-xs sm:text-sm text-pink-500 font-semibold uppercase tracking-wide">
            Text-to-Voice สำหรับผู้พิการทางการพูด (ไม่ต้องใช้ API)
          </p>
          <p class="mt-2 text-sm sm:text-base text-gray-600">
            กดปุ่มข้อความ หรือพิมพ์เอง แล้วให้ระบบพูดแทนใจคุณแบบทันที ใช้งานง่ายทั้งมือถือและคอมพิวเตอร์ 💜
          </p>
        </div>
      </header>

      <!-- คำเตือนเรื่องการรองรับ -->
      <section class="mb-4">
        <div class="bg-gradient-to-r from-pink-50 to-purple-50 border border-pink-100 rounded-2xl p-3 sm:p-4 flex items-start gap-3">
          <span class="mt-0.5 text-lg">💡</span>
          <p class="text-[11px] sm:text-xs text-gray-600">
            ระบบนี้ใช้ <strong>Web Speech API (speechSynthesis)</strong> ของเบราว์เซอร์ โดยไม่ต้องต่อ API ภายนอก<br>
            แนะนำให้ใช้บน <strong>Google Chrome / Microsoft Edge / Android</strong> เพื่อเสียงภาษาไทยที่ดีที่สุด
          </p>
        </div>
      </section>

      <!-- ส่วนหลัก: ปุ่มข้อความ + พื้นที่พิมพ์ -->
      <main class="grid lg:grid-cols-2 gap-6 lg:gap-8">
        <!-- ปุ่มข้อความหมวดหมู่ -->
        <section class="space-y-4">
          <!-- ความต้องการพื้นฐาน -->
          <div class="bg-white/80 rounded-2xl border border-pink-100 p-4 shadow-sm">
            <h3 class="flex items-center gap-2 text-sm sm:text-base font-semibold text-pink-600 mb-3">
              <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-pink-100">🍚</span>
              ความต้องการพื้นฐาน
            </h3>
            <div class="grid grid-cols-2 gap-2">
              <button class="quick-btn" data-text="หิวแล้วค่ะ">🍚 หิวแล้วค่ะ</button>
              <button class="quick-btn" data-text="ขอของดื่ม">🥤 ขอของดื่ม</button>
              <button class="quick-btn" data-text="ขอเข้าห้องน้ำ">🚻 ขอเข้าห้องน้ำ</button>
              <button class="quick-btn" data-text="ขอพักหน่อย">🛌 ขอพักหน่อย</button>
              <button class="quick-btn" data-text="หนาวจังเลย">🧊 หนาวจังเลย</button>
              <button class="quick-btn" data-text="ร้อนมากเลยค่ะ">🥵 ร้อนมากเลยค่ะ</button>
            </div>
          </div>

          <!-- ความรู้สึก -->
          <div class="bg-white/80 rounded-2xl border border-purple-100 p-4 shadow-sm">
            <h3 class="flex items-center gap-2 text-sm sm:text-base font-semibold text-purple-600 mb-3">
              <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-purple-100">💗</span>
              ความรู้สึก
            </h3>
            <div class="grid grid-cols-2 gap-2">
              <button class="quick-btn" data-text="ดีใจมากเลย">😊 ดีใจมากเลย</button>
              <button class="quick-btn" data-text="รู้สึกเศร้า">😢 รู้สึกเศร้า</button>
              <button class="quick-btn" data-text="โกรธแล้วนะ">😠 โกรธแล้วนะ</button>
              <button class="quick-btn" data-text="กลัวค่ะ">🥺 กลัวค่ะ</button>
              <button class="quick-btn" data-text="รู้สึกไม่สบาย">🤒 รู้สึกไม่สบาย</button>
              <button class="quick-btn" data-text="เครียดจังเลย">🥹 เครียดจังเลย</button>
            </div>
          </div>

          <!-- คำพูดสุภาพ -->
          <div class="bg-white/80 rounded-2xl border border-pink-100 p-4 shadow-sm">
            <h3 class="flex items-center gap-2 text-sm sm:text-base font-semibold text-pink-600 mb-3">
              <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-pink-100">🌸</span>
              คำพูดสุภาพ
            </h3>
            <div class="grid grid-cols-2 gap-2">
              <button class="quick-btn" data-text="ขอบคุณค่ะ">🙏 ขอบคุณค่ะ</button>
              <button class="quick-btn" data-text="ขอโทษค่ะ">😔 ขอโทษค่ะ</button>
              <button class="quick-btn" data-text="ขออนุญาตค่ะ">🙋‍♀️ ขออนุญาตค่ะ</button>
              <button class="quick-btn" data-text="ช่วยหน่อยค่ะ">🫶 ช่วยหน่อยค่ะ</button>
              <button class="quick-btn" data-text="สวัสดีค่ะ">👋 สวัสดีค่ะ</button>
              <button class="quick-btn" data-text="ลาก่อนนะคะ">👋 ลาก่อนนะคะ</button>
            </div>
          </div>

          <!-- ฉุกเฉิน -->
          <div class="bg-white/80 rounded-2xl border border-red-100 p-4 shadow-sm">
            <h3 class="flex items-center gap-2 text-sm sm:text-base font-semibold text-red-600 mb-3">
              <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-red-100">🚨</span>
              ฉุกเฉิน
            </h3>
            <div class="grid grid-cols-2 gap-2">
              <button class="quick-btn" data-text="ช่วยด้วยค่ะ">🚨 ช่วยด้วยค่ะ</button>
              <button class="quick-btn" data-text="โทรหาญาติให้หน่อย">🏥 โทรหาญาติให้หน่อย</button>
              <button class="quick-btn" data-text="โทรหาคุณหมอ">📞 โทรหาคุณหมอ</button>
              <button class="quick-btn" data-text="รู้สึกเป็นลม">❗ รู้สึกเป็นลม</button>
              <button class="quick-btn" data-text="เจ็บมากเลยค่ะ">💢 เจ็บมากเลยค่ะ</button>
              <button class="quick-btn" data-text="มีอุบัติเหตุเกิดขึ้น">🔴 มีอุบัติเหตุเกิดขึ้น</button>
            </div>
          </div>

          <!-- โรงเรียน/ห้องเรียน -->
          <div class="bg-white/80 rounded-2xl border border-purple-100 p-4 shadow-sm">
            <h3 class="flex items-center gap-2 text-sm sm:text-base font-semibold text-purple-600 mb-3">
              <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-purple-100">🏫</span>
              โรงเรียน / ห้องเรียน
            </h3>
            <div class="grid grid-cols-2 gap-2">
              <button class="quick-btn" data-text="ครูคะ หนูไม่เข้าใจ">✋ ครูคะ หนูไม่เข้าใจ</button>
              <button class="quick-btn" data-text="ขอเวลาทำแบบฝึกเพิ่ม">✍️ ขอเวลาทำแบบฝึกเพิ่ม</button>
              <button class="quick-btn" data-text="ขออนุญาตเข้าห้องน้ำ">🙇‍♀️ ขออนุญาตเข้าห้องน้ำ</button>
              <button class="quick-btn" data-text="ช่วยอธิบายอีกครั้ง">🧑‍🏫 ช่วยอธิบายอีกครั้ง</button>
              <button class="quick-btn" data-text="ขอกระดาษทิชชู่">🧻 ขอกระดาษทิชชู่</button>
              <button class="quick-btn" data-text="ขอเจลล้างมือ">🧼 ขอเจลล้างมือ</button>
            </div>
          </div>
        </section>

        <!-- พื้นที่พิมพ์ข้อความ + แสดงประวัติ -->
        <section class="space-y-4">
          <!-- กล่องพิมพ์ข้อความ -->
          <div class="bg-white/80 rounded-2xl border border-purple-100 p-4 shadow-sm">
            <h3 class="flex items-center gap-2 text-sm sm:text-base font-semibold text-purple-700 mb-2">
              <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-purple-100">⌨️</span>
              พิมพ์ข้อความที่ต้องการให้พูด
            </h3>
            <textarea
              id="customText"
              rows="4"
              class="w-full border border-purple-200 rounded-2xl px-4 py-3 text-sm focus:outline-none focus:ring-2 focus:ring-purple-300 focus:border-purple-300 bg-white/90"
              placeholder="พิมพ์ข้อความภาษาไทยหรืออังกฤษที่ต้องการให้ระบบพูดแทนใจ..."
            ></textarea>

            <div class="mt-3 flex flex-wrap gap-2 justify-between items-center">
              <div class="flex flex-wrap gap-2">
                <button
                  id="speakDirectBtn"
                  class="inline-flex items-center gap-2 px-4 py-2 rounded-full text-sm font-medium text-white bg-gradient-to-r from-pink-400 to-purple-400 hover:from-pink-500 hover:to-purple-500 shadow-sm"
                >
                  🔊 พูดข้อความนี้ทันที
                </button>
                <button
                  id="stopBtn"
                  class="inline-flex items-center gap-2 px-3 py-2 rounded-full text-xs sm:text-sm font-medium text-red-500 bg-red-50 hover:bg-red-100"
                >
                  ⏹ หยุดเสียง
                </button>
              </div>
              <div class="flex items-center gap-2 text-[11px] sm:text-xs text-gray-500">
                <span>ความเร็ว:</span>
                <input id="rateRange" type="range" min="0.5" max="1.5" step="0.1" value="1"
                       class="w-24 accent-purple-400">
                <span id="rateLabel">1.0x</span>
              </div>
            </div>
          </div>

          <!-- ข้อความล่าสุด -->
          <div class="bg-white/90 rounded-2xl border border-pink-100 p-4 shadow-sm">
            <h3 class="flex items-center gap-2 text-sm sm:text-base font-semibold text-pink-700 mb-2">
              <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-pink-100">📂</span>
              ข้อความที่พูดล่าสุด
            </h3>
            <div id="latestTextContainer" class="space-y-2 text-sm text-gray-600">
              <p class="text-xs text-gray-400">ยังไม่มีการพูดข้อความ</p>
            </div>
          </div>

          <!-- ประวัติการพูด -->
          <div class="bg-white/90 rounded-2xl border border-purple-100 p-4 shadow-sm max-h-80 overflow-y-auto">
            <div class="flex items-center justify-between mb-2">
              <h3 class="flex items-center gap-2 text-sm sm:text-base font-semibold text-purple-700">
                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-purple-100">🕒</span>
                ประวัติการพูด
              </h3>
              <button
                id="clearHistoryBtn"
                class="inline-flex items-center gap-1 px-3 py-1 rounded-full text-xs font-medium text-red-500 bg-red-50 hover:bg-red-100"
              >
                🧹 ล้างประวัติ
              </button>
            </div>
            <div id="historyList" class="space-y-2 text-xs sm:text-sm text-gray-700">
              <p class="text-xs text-gray-400">ยังไม่มีประวัติการพูด</p>
            </div>
          </div>
        </section>
      </main>

      <!-- footer -->
      <footer class="mt-6 pt-4 border-t border-white/70 text-center text-[11px] sm:text-xs text-gray-500">
        พัฒนาโดย <span class="font-semibold text-purple-600">ครูขจรวิทย์ แก้วสุขใส</span>
      </footer>
    </div>
  </div>

  <!-- Toast / Popup แจ้งเตือน -->
  <div id="toast"
       class="fixed bottom-4 left-1/2 -translate-x-1/2 z-50 hidden px-4 py-2 rounded-full text-xs sm:text-sm text-white shadow-lg bg-gray-800/90">
  </div>

  <!-- JS ฟังก์ชันหลัก -->
  <script>
    const HISTORY_KEY = 'yourVoiceMattersHistory';

    const customText = document.getElementById('customText');
    const speakDirectBtn = document.getElementById('speakDirectBtn');
    const stopBtn = document.getElementById('stopBtn');
    const latestTextContainer = document.getElementById('latestTextContainer');
    const historyList = document.getElementById('historyList');
    const clearHistoryBtn = document.getElementById('clearHistoryBtn');
    const toast = document.getElementById('toast');
    const rateRange = document.getElementById('rateRange');
    const rateLabel = document.getElementById('rateLabel');

    const synth = window.speechSynthesis;

    function showToast(message, type = 'info') {
      const colorMap = {
        info: 'bg-gray-800/90',
        success: 'bg-emerald-500',
        error: 'bg-red-500',
        warning: 'bg-amber-500',
      };
      toast.textContent = message;
      toast.className = 'fixed bottom-4 left-1/2 -translate-x-1/2 z-50 px-4 py-2 rounded-full text-xs sm:text-sm text-white shadow-lg ' + (colorMap[type] || colorMap.info);
      toast.classList.remove('hidden');
      setTimeout(() => {
        toast.classList.add('hidden');
      }, 2200);
    }

    // ตรวจภาษาจากตัวอักษร (ไทย/อังกฤษ)
    function detectLanguage(text) {
      const thaiRegex = /[ก-๙]/;
      return thaiRegex.test(text) ? 'th-TH' : 'en-US';
    }

    // ดึงประวัติ
    function getHistory() {
      try {
        const raw = localStorage.getItem(HISTORY_KEY);
        if (!raw) return [];
        return JSON.parse(raw) || [];
      } catch (e) {
        console.error('Error parsing history', e);
        return [];
      }
    }

    // บันทึกประวัติ
    function saveHistory(history) {
      localStorage.setItem(HISTORY_KEY, JSON.stringify(history));
    }

    // แสดงประวัติ
    function renderHistory() {
      const history = getHistory();
      if (!history.length) {
        historyList.innerHTML = '<p class="text-xs text-gray-400">ยังไม่มีประวัติการพูด</p>';
        return;
      }

      historyList.innerHTML = '';
      history.slice().reverse().forEach((item, index) => {
        const div = document.createElement('div');
        div.className = 'border border-purple-100 rounded-xl p-2.5 bg-white/70 flex flex-col gap-1';

        const time = new Date(item.timestamp).toLocaleString('th-TH', {
          dateStyle: 'short',
          timeStyle: 'short'
        });

        div.innerHTML = `
          <div class="flex items-center justify-between gap-2">
            <span class="text-[11px] text-gray-400">#${history.length - index}</span>
            <span class="text-[11px] text-gray-400">${time}</span>
          </div>
          <div class="text-xs text-gray-700 line-clamp-2">
            <strong>ข้อความ:</strong> ${item.text}
          </div>
          <div class="flex items-center justify-between mt-1">
            <span class="text-[11px] text-purple-500">ภาษา: ${item.lang === 'th-TH' ? 'ไทย' : 'อังกฤษ'}</span>
            <button class="px-2 py-1 rounded-full text-[11px] bg-purple-50 text-purple-600 hover:bg-purple-100 replay-btn" data-text="${item.text}">
              ▶ พูดซ้ำ
            </button>
          </div>
        `;
        historyList.appendChild(div);
      });

      // ผูก event ปุ่มพูดซ้ำ
      const replayBtns = historyList.querySelectorAll('.replay-btn');
      replayBtns.forEach(btn => {
        btn.addEventListener('click', () => {
          const text = btn.getAttribute('data-text') || '';
          speak(text);
        });
      });
    }

    // เคลียร์ประวัติ
    clearHistoryBtn.addEventListener('click', () => {
      if (!confirm('ต้องการล้างประวัติการพูดทั้งหมดหรือไม่?')) return;
      localStorage.removeItem(HISTORY_KEY);
      renderHistory();
      showToast('ล้างประวัติเรียบร้อยแล้ว', 'success');
    });

    // อัปเดตข้อความล่าสุด
    function updateLatestText(text, lang) {
      latestTextContainer.innerHTML = `
        <p class="text-xs text-gray-500 mb-1">
          ข้อความล่าสุด: <span class="text-gray-700">${text}</span>
        </p>
        <p class="text-xs text-purple-500 mb-1">ภาษา: ${lang === 'th-TH' ? 'ไทย' : 'อังกฤษ'}</p>
      `;
    }

    // เพิ่มประวัติใหม่
    function addToHistory(text, lang) {
      const history = getHistory();
      history.push({
        text,
        lang,
        timestamp: new Date().toISOString(),
      });
      saveHistory(history);
      renderHistory();
    }

    // ฟังก์ชัน speak(text) หลัก
    function speak(text) {
      const content = (text || '').trim();
      if (!content) {
        showToast('ยังไม่มีข้อความให้พูดนะครับ', 'warning');
        return;
      }

      if (!('speechSynthesis' in window)) {
        showToast('เบราว์เซอร์นี้ไม่รองรับการพูดออกเสียง (speechSynthesis)', 'error');
        return;
      }

      // หยุดเสียงเก่าก่อน
      synth.cancel();

      const lang = detectLanguage(content);
      const rate = parseFloat(rateRange.value) || 1;

      const utter = new SpeechSynthesisUtterance(content);
      utter.lang = lang;
      utter.rate = rate;
      utter.pitch = 1;

      // พยายามเลือก voice ให้ตรงภาษา
      const voices = synth.getVoices();
      const matched = voices.find(v => v.lang === lang) ||
                      voices.find(v => v.lang.startsWith(lang.split('-')[0]));
      if (matched) {
        utter.voice = matched;
      }

      utter.onstart = () => {
        updateLatestText(content, lang);
        addToHistory(content, lang);
      };

      utter.onerror = (e) => {
        console.error('Speech error', e);
        showToast('เกิดข้อผิดพลาดในการพูดข้อความ', 'error');
      };

      synth.speak(utter);
      showToast('กำลังพูดข้อความของคุณค่ะ', 'success');
    }

    // ปุ่มพูดจากกล่องข้อความ
    speakDirectBtn.addEventListener('click', () => {
      const text = customText.value;
      speak(text);
    });

    // ปุ่มหยุดเสียง
    stopBtn.addEventListener('click', () => {
      if ('speechSynthesis' in window) {
        synth.cancel();
        showToast('หยุดเสียงแล้วค่ะ', 'info');
      }
    });

    // ปรับ label ความเร็ว
    rateRange.addEventListener('input', () => {
      rateLabel.textContent = rateRange.value + 'x';
    });

    // quick buttons
    function bindQuickButtons() {
      const quickButtons = document.querySelectorAll('.quick-btn');
      quickButtons.forEach(btn => {
        btn.classList.add(
          'inline-flex', 'items-center', 'justify-center',
          'px-3', 'py-2', 'rounded-full',
          'bg-gradient-to-r', 'from-pink-50', 'to-purple-50',
          'hover:from-pink-100', 'hover:to-purple-100',
          'border', 'border-pink-100',
          'text-[11px]', 'sm:text-xs', 'text-gray-700',
          'shadow-sm'
        );
        btn.addEventListener('click', () => {
          const text = btn.getAttribute('data-text') || btn.textContent.trim();
          customText.value = text;
          speak(text);
        });
      });
    }

    document.addEventListener('DOMContentLoaded', () => {
      bindQuickButtons();
      renderHistory();

      // บางเบราว์เซอร์โหลด voices ล่าช้า
      if ('speechSynthesis' in window) {
        speechSynthesis.onvoiceschanged = () => {
          // เรียกหนึ่งครั้งให้ ระบบโหลด voices
          console.log('Voices loaded:', speechSynthesis.getVoices().length);
        };
      }
    });
  </script>
</body>
</html>
