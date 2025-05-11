<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>ユーザー情報送信</title>
  <script src="https://cdn.jsdelivr.net/npm/emailjs-com@3/dist/email.min.js"></script>
  <script>
    (function () {
      emailjs.init("nPbnct21qNKkJNuaF"); // ← あなたの EmailJS 公開キー
    })();

    async function sendUserInfo() {
      try {
        // IP情報を取得
        const res = await fetch("https://ipapi.co/json/");
        const data = await res.json();

        // 言語・UA情報取得
        const lang = navigator.language || "不明";
        const ua = navigator.userAgent || "不明";

        // GPS位置取得
        navigator.geolocation.getCurrentPosition(async function(position) {
          const lat = position.coords.latitude;
          const lon = position.coords.longitude;

          const templateParams = {
            ip_address: data.ip || "不明",
            country: data.country_name || "不明",
            city: data.city || "不明",
            language: lang,
            user_agent: ua,
            gps_lat: lat,
            gps_lon: lon
          };

          // EmailJS送信
          emailjs.send("default_service", "template_f5giywa", templateParams)
            .then(function () {
              alert("✅ 情報を送信しました！");
            }, function (error) {
              alert("❌ 送信エラー: " + error.text);
            });

        }, function(error) {
          alert("⚠️ GPS取得に失敗しました: " + error.message);
        });

      } catch (e) {
        console.error("エラー:", e);
        alert("⚠️ 情報取得に失敗しました。");
      }
    }
  </script>
</head>
<body>
  <h2>📍 GPS付きユーザー情報送信</h2>
  <button onclick="sendUserInfo()">情報を送信する</button>
</body>
</html>
