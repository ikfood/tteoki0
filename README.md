<!doctype html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#18aada">
  <meta name="description" content="아이케이푸드 디지털팀 김우영 주임 모바일 명함">
  <title>김우영 주임 | IK FOOD</title>

  <style>
    :root {
      --blue: #18aada;
      --deep: #1779ae;
      --ink: #182c3a;
      --muted: #7a8c98;
      --line: #e1edf3;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      color: var(--ink);
      background: #eaf4f8;
      font-family:
        -apple-system, BlinkMacSystemFont,
        "Apple SD Gothic Neo", "Malgun Gothic",
        Arial, sans-serif;
      -webkit-font-smoothing: antialiased;
    }

    button, a {
      font: inherit;
      -webkit-tap-highlight-color: transparent;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    button {
      cursor: pointer;
    }

    button:disabled {
      cursor: default;
    }

    .card {
      max-width: 440px;
      margin: 44px auto;
      overflow: hidden;
      background: white;
      border: 1px solid white;
      border-radius: 30px;
      box-shadow: 0 20px 70px #204a6412;
    }

    .header {
      padding: 35px 28px 29px;
      text-align: center;
    }

    .eyebrow {
      margin: 0;
      color: var(--deep);
      font-size: 10px;
      font-weight: 650;
      letter-spacing: 2px;
    }

    .logo {
      display: flex;
      align-items: center;
      justify-content: center;
      width: 140px;
      height: 140px;
      margin: 24px auto 22px;
      overflow: hidden;
      background: white;
      border: 1px solid #dfedf3;
      border-radius: 50%;
      box-shadow: 0 6px 24px #137ead08;
    }

    .logo img {
      display: block;
      width: 108px;
      height: auto;
    }

    .company {
      color: #36586d;
      font-size: 15px;
      font-weight: 650;
      letter-spacing: -0.5px;
    }

    .person {
      display: flex;
      align-items: baseline;
      justify-content: center;
      gap: 11px;
      margin-top: 14px;
    }

    h1 {
      margin: 0;
      font-size: 31px;
      font-weight: 750;
      line-height: 1.3;
      letter-spacing: 2px;
    }

    .position {
      color: var(--muted);
      font-size: 13px;
    }

    .intro {
      margin: 13px 0 0;
      color: #8d9ea8;
      font-size: 12px;
      letter-spacing: 0.2px;
    }

    .content {
      padding: 27px 27px 22px;
      background: #f4f9fc;
      border-radius: 28px 28px 0 0;
    }

    .shortcuts {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
      margin-bottom: 29px;
    }

    .shortcut {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 0;
      color: #3f5b6e;
      text-align: center;
      background: none;
      border: 0;
    }

    .circle {
      display: flex;
      align-items: center;
      justify-content: center;
      width: 58px;
      height: 58px;
      color: white;
      background: var(--blue);
      border-radius: 50%;
      box-shadow: 0 5px 12px #19aada15;
    }

    .mail .circle {
      background: #228dbb;
    }

    .kakao .circle {
      background: #1779ae;
    }

    .kakao.pending .circle {
      color: #839eae;
      background: #e2edf3;
      box-shadow: none;
    }

    .shortcut strong {
      margin-top: 10px;
      font-size: 12px;
      font-weight: 650;
    }

    .shortcut small {
      min-height: 12px;
      margin-top: 4px;
      color: #91a4b1;
      font-size: 9px;
    }

    svg {
      width: 23px;
      height: 23px;
      fill: none;
      stroke: currentColor;
      stroke-width: 1.8;
      stroke-linecap: round;
      stroke-linejoin: round;
    }

    .info {
      border-top: 1px solid var(--line);
    }

    .row {
      display: grid;
      grid-template-columns: 60px 1fr 14px;
      align-items: start;
      gap: 10px;
      padding: 17px 0;
      border-bottom: 1px solid var(--line);
    }

    .label {
      padding-top: 3px;
      color: var(--deep);
      font-size: 10px;
      font-weight: 700;
      letter-spacing: 1px;
    }

    .value {
      color: #3f586a;
      font-size: 13px;
      line-height: 1.65;
      overflow-wrap: anywhere;
    }

    .arrow {
      margin-top: 2px;
      color: #96acba;
      font-size: 13px;
    }

    .address .value {
      font-size: 12px;
    }

    .fax {
      padding: 14px 0;
    }

    .fax .value {
      color: #7e929f;
      font-size: 12px;
    }

    .links {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 9px;
      margin-top: 22px;
    }

    .links a {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 13px 10px;
      color: #557489;
      font-size: 11px;
      font-weight: 600;
      background: white;
      border: 1px solid #d6e6ef;
      border-radius: 11px;
    }

    .actions {
      display: grid;
      grid-template-columns: 1fr 46px;
      gap: 9px;
      margin-top: 20px;
    }

    .actions button {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      height: 46px;
      color: var(--deep);
      font-size: 12px;
      font-weight: 650;
      background: white;
      border: 1px solid #d4e6f0;
      border-radius: 12px;
    }

    .actions .save {
      color: white;
      background: var(--blue);
      border-color: var(--blue);
    }

    .actions svg {
      width: 18px;
      height: 18px;
    }

    .footer {
      padding-top: 23px;
      color: #9bafbc;
      font-size: 9px;
      text-align: center;
      letter-spacing: 1px;
    }

    .toast {
      position: fixed;
      bottom: 22px;
      left: 50%;
      z-index: 10;
      display: none;
      max-width: 90vw;
      padding: 13px 20px;
      color: white;
      font-size: 12px;
      line-height: 1.5;
      background: #203c50;
      border-radius: 20px;
      transform: translateX(-50%);
    }

    .toast.show {
      display: block;
    }

    :focus-visible {
      outline: 3px solid #176f9f;
      outline-offset: 5px;
    }

    @media (max-width: 500px) {
      body {
        background: white;
      }

      .card {
        min-height: 100dvh;
        margin: 0 auto;
        border: 0;
        border-radius: 0;
        box-shadow: none;
      }

      .header {
        padding-top: 30px;
      }

      .content {
        min-height: calc(100dvh - 313px);
      }
    }

    @media (max-width: 350px) {
      .content {
        padding-right: 21px;
        padding-left: 21px;
      }

      .row {
        grid-template-columns: 52px 1fr 12px;
        gap: 6px;
      }

      .value {
        font-size: 12px;
      }

      .person {
        gap: 8px;
      }

      h1 {
        font-size: 28px;
      }
    }
  </style>
</head>

<body>
  <main class="card">
    <header class="header">
      <p class="eyebrow">IK FOOD · DIGITAL BUSINESS CARD</p>

      <div class="logo">
        <!-- 로고를 GitHub에 함께 올리면 src="ikfood-logo.png"로 변경 -->
        <img
          src="https://hotissue-mobile-card.agilevine13.chatgpt.site/ikfood-logo.png"
          alt="IK FOOD 아이케이푸드 로고"
        >
      </div>

      <div class="company">(주)아이케이푸드</div>

      <div class="person">
        <h1>김우영</h1>
        <span class="position">디지털팀 · 주임</span>
      </div>

      <p class="intro">HMR · 밀떡 · 쌀떡 · 면류</p>
    </header>

    <section class="content" aria-label="연락처 및 회사 정보">
      <nav class="shortcuts" aria-label="연락 바로가기">
        <a class="shortcut" href="tel:01084533351">
          <span class="circle">
            <svg viewBox="0 0 24 24" aria-hidden="true">
              <path d="m7 3 3 5-2 2c1.4 2.7 3.3 4.6 6 6l2-2 5 3c-1 5-5 5-9 3C6 17 2 11 3 6c.4-2 1.7-3 4-3Z"/>
            </svg>
          </span>
          <strong>통화</strong>
          <small>전화하기</small>
        </a>

        <a class="shortcut mail" href="mailto:wooy6456@naver.com">
          <span class="circle">
            <svg viewBox="0 0 24 24" aria-hidden="true">
              <rect x="3" y="5" width="18" height="14" rx="2"/>
              <path d="m3 6 9 7 9-7"/>
            </svg>
          </span>
          <strong>메일</strong>
          <small>메일 보내기</small>
        </a>

        <button
          class="shortcut kakao pending"
          id="kakao"
          type="button"
          disabled
          aria-label="카카오톡 연결 준비 중"
        >
          <span class="circle">
            <svg viewBox="0 0 24 24" aria-hidden="true">
              <path d="M12 3c-5.5 0-10 3.5-10 7.8 0 2.8 1.8 5.2 4.5 6.6l-1 3.8 4.2-2.8c.7.1 1.5.2 2.3.2 5.5 0 10-3.5 10-7.8S17.5 3 12 3Z"/>
              <path d="M7 10.7h.1m4.9 0h.1m4.9 0h.1" stroke-width="2.7"/>
            </svg>
          </span>
          <strong>카카오톡</strong>
          <small id="kakao-label">연결 준비 중</small>
        </button>
      </nav>

      <div class="info">
        <a class="row" href="tel:01084533351">
          <span class="label">MOBILE</span>
          <span class="value">010-8453-3351</span>
          <span class="arrow">↗</span>
        </a>

        <a class="row" href="mailto:wooy6456@naver.com">
          <span class="label">EMAIL</span>
          <span class="value">wooy6456@naver.com</span>
          <span class="arrow">↗</span>
        </a>

        <a class="row" href="tel:07042949594">
          <span class="label">TEL</span>
          <span class="value">070-4294-9594</span>
          <span class="arrow">↗</span>
        </a>

        <div class="row fax">
          <span class="label">FAX</span>
          <span class="value">032-715-7790</span>
        </div>

        <div class="row address">
          <span class="label">ADDRESS</span>
          <span class="value">
            경기도 부천시 오정구<br>
            삼작로 115번길 65 (삼정동)<br>
            우편번호 14451
          </span>
        </div>
      </div>

      <div class="links">
        <a
          href="https://www.ik-food.com"
          target="_blank"
          rel="noopener noreferrer"
        >
          회사 홈페이지 <span>↗</span>
        </a>

        <a
          href="https://www.instagram.com/hotissueshop_official/"
          target="_blank"
          rel="noopener noreferrer"
        >
          핫이슈샵 인스타그램 <span>↗</span>
        </a>
      </div>

      <div class="actions">
        <button class="save" id="save" type="button">
          <svg viewBox="0 0 24 24" aria-hidden="true">
            <path d="M12 3v12m-5-5 5 5 5-5M4 16v5h16v-5"/>
          </svg>
          연락처 저장
        </button>

        <button id="share" type="button" aria-label="명함 공유">
          <svg viewBox="0 0 24 24" aria-hidden="true">
            <path d="M12 16V3m-4 4 4-4 4 4M5 12v9h14v-9"/>
          </svg>
        </button>
      </div>

      <footer class="footer">IK FOOD © 2026</footer>
    </section>
  </main>

  <div class="toast" id="toast" role="status"></div>

  <script>
    // 카카오톡 채널 또는 오픈채팅 링크를 따옴표 안에 입력하세요.
    const KAKAO_URL = "";

    const kakaoButton = document.getElementById("kakao");

    if (KAKAO_URL.trim()) {
      try {
        const kakaoUrl = new URL(KAKAO_URL);

        if (kakaoUrl.protocol === "https:") {
          kakaoButton.disabled = false;
          kakaoButton.classList.remove("pending");
          kakaoButton.setAttribute("aria-label", "카카오톡으로 대화하기");

          document.getElementById("kakao-label").textContent = "대화하기";

          kakaoButton.addEventListener("click", () => {
            window.open(kakaoUrl.href, "_blank", "noopener,noreferrer");
          });
        }
      } catch {
        console.warn("카카오톡 링크를 확인해주세요.");
      }
    }

    const toast = document.getElementById("toast");
    let toastTimer;

    function notify(message) {
      toast.textContent = message;
      toast.classList.add("show");

      clearTimeout(toastTimer);
      toastTimer = setTimeout(() => {
        toast.classList.remove("show");
      }, 3500);
    }

    document.getElementById("save").addEventListener("click", () => {
      const vcard = [
        "BEGIN:VCARD",
        "VERSION:3.0",
        "FN:김우영",
        "N:김우영;;;;",
        "ORG:(주)아이케이푸드",
        "TITLE:디지털팀 주임",
        "TEL;TYPE=CELL:01084533351",
        "TEL;TYPE=WORK:07042949594",
        "TEL;TYPE=FAX:0327157790",
        "EMAIL:wooy6456@naver.com",
        "ADR;TYPE=WORK:;;삼작로 115번길 65 (삼정동);부천시 오정구;경기도;14451;대한민국",
        "URL:https://www.ik-food.com",
        "END:VCARD"
      ].join("\r\n");

      const blob = new Blob([vcard], {
        type: "text/vcard;charset=utf-8"
      });

      const url = URL.createObjectURL(blob);
      const link = document.createElement("a");

      link.href = url;
      link.download = "아이케이푸드_김우영.vcf";

      document.body.appendChild(link);
      link.click();
      link.remove();

      setTimeout(() => URL.revokeObjectURL(url), 1000);

      notify("다운로드한 연락처 파일을 열어 저장해주세요.");
    });

    document.getElementById("share").addEventListener("click", async () => {
      if (location.protocol === "file:") {
        notify("웹에 업로드한 뒤 명함 링크를 공유해주세요.");
        return;
      }

      const pageUrl = new URL(location.href);
      pageUrl.hash = "";
      pageUrl.search = "";

      try {
        if (navigator.share) {
          await navigator.share({
            title: "김우영 주임 | IK FOOD",
            url: pageUrl.href
          });
        } else if (navigator.clipboard) {
          await navigator.clipboard.writeText(pageUrl.href);
          notify("명함 링크를 복사했습니다.");
        } else {
          window.prompt("명함 링크를 복사해주세요.", pageUrl.href);
        }
      } catch (error) {
        if (error.name !== "AbortError") {
          window.prompt("명함 링크를 복사해주세요.", pageUrl.href);
        }
      }
    });
  </script>
</body>
</html>
