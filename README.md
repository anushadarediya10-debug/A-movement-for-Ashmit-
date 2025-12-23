# A-movement-for-Ashmit-

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>A Small Moment for Ashmit</title>

<style>
body {
  background: #0b0f14;
  color: #e6edf3;
  font-family: Georgia, serif;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  text-align: center;
}

.box {
  max-width: 600px;
  padding: 30px;
}

#text {
  font-size: 22px;
  line-height: 1.6;
}
</style>
</head>

<body>

<div class="box">
  <p id="text"></p>
</div>

<script>
const message = `
Ashmit,

You turned 29 today.

We’ve known each other for only two months.
That’s not a long time…
but somehow, it feels important.

This page isn’t fancy.
It’s just a small moment I wanted to save —
a reminder that today mattered,
and so did you.

Happy Birthday 🤍
— Anusha
`;

let i = 0;
function typeEffect() {
  if (i < message.length) {
    document.getElementById("text").innerHTML +=
      message.charAt(i) === "\n" ? "<br>" : message.charAt(i);
    i++;
    setTimeout(typeEffect, 45);
  }
}
typeEffect();
</script>

</body>
</html>
