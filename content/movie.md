---
title: "Movie"
date: 2019-09-16T12:35:20+08:00
draft: false
---
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="referrer" content="never">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>bmdb</title>
  <style>
    body {
      margin: 50px 0;
      font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
      font-weight: 400;
      font-size: 16px;
      line-height: 1.7;
      color: #333;
      -webkit-size-adjust: 100%;
    }

    .container {
      width: 1000px;
      margin: auto
    }

    @media screen and (max-width:768px) {
      .container {
        width: auto;
        margin-left: 15px;
        margin-right: 15px;
      }
    }
  </style>
</head>
<body>
  <div class="container"></div>
  <script src="https://cdn.jsdelivr.net/npm/jquery@3.3.1/dist/jquery.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/jquery@3.3.1/dist/jquery.min.js"></script>
  <script src="https://cdn.jsdelivr.net/gh/iMuFeng/bmdb@1.2.1/dist/Bmdb.min.js"></script>
</body>
<script>
  new Bmdb({
    type: 'movies',
    selector: '.container',
    cache: true,
    showCategories: true,
    noMoreText: '没有更多数据了',
    secret: '7bf4205a0a62d00409f3cd70b0736e1a11a9a6a60f7231567f056819787b8096'
  })
</script>
</html>
