<!DOCTYPE html>
<html>
<head>
<style>
body {
  background: #111;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
.flower {
  font-size: 100px;
  animation: bloom 2s infinite;
}
@keyframes bloom {
  0% { transform: scale(0.5) rotate(0deg); }
  50% { transform: scale(1.2) rotate(10deg); }
  100% { transform: scale(1) rotate(0deg); }
}
</style>
</head>
<body>
  <div class="flower">🌸</div>
</body>
</html>