<!DOCTYPE html>
<html>
<head>
  <title>مزحة إشعار</title>
</head>
<body>
  <h1>افتح الإشعارات وشوف المفاجأة!</h1>
  <script>
    if ('Notification' in window) {
      Notification.requestPermission().then(permission => {
        if (permission === 'granted') {
          new Notification('تم اختراق تلفونك!', {
            body: 'لا تخاف، هاي بس مزحة من صهيب 😄',
            icon: 'https://example.com/icon.png' // تقدر تحط رابط أي صورة صغيرة
          });
        }
      });
    } else {
      alert('جهازك ما يدعم الإشعارات.');
    }
  </script>
</body>
</html>
