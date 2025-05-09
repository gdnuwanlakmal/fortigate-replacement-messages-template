# FortiGate Replacement Message Template
FortiGate Replacement Messages are customizable templates shown to users in response to various system or security events — such as web filtering blocks, antivirus alerts, SSL inspection notices, etc.

### FortiGuard Block Page Template

``` shell
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Access Blocked</title>
  <style>
    /* Basic reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      height: 100vh;
      font-family: 'Arial', sans-serif;
      background: linear-gradient(to right, #05000a, #1a0026);
      color: #e0e0e0;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      overflow: auto;
      padding: 20px;
    }

    .container {
      background: #0f0f0f;
      padding: 40px 20px;
      border-radius: 15px;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.8);
      max-width: 600px;
      width: 100%;
      animation: fadeIn 1.5s ease-in-out;
    }

    .logo {
      margin-bottom: 20px;
    }

    .logo img {
      width: 100px;
      height: auto;
    }

    h1 {
      font-size: 30px;
      margin-bottom: 15px;
      color: #ff4d4d;
    }

    p {
      font-size: 16px;
      margin-bottom: 20px;
      line-height: 1.6;
      text-align: center;
      width: 100%;
    }

    .contact-info {
      font-size: 14px;
      color: #b3b3b3;
    }

    /* Table styles */
    table {
      width: 100%;
      margin: 20px 0;
      border-collapse: collapse;
      color: #e0e0e0;
      table-layout: fixed;
    }

    table,
    th,
    td {
      border: 1px solid #444444;
    }

    th,
    td {
      padding: 12px;
      text-align: left;
      word-wrap: break-word;
    }

    th {
      background-color: #444444;
      color: #ffffff;
    }

    td {
      background-color: #2e2e2e;
    }

    @keyframes fadeIn {
      0% {
        opacity: 0;
      }

      100% {
        opacity: 1;
      }
    }

    .link {
      color: #ff4d4d;
      text-decoration: none;
      font-weight: bold;
    }

    .link:hover {
      text-decoration: underline;
      color: #ff6666;
    }

    .highlight {
      color: #ff4d4d;
      font-weight: bold;
    }
  </style>
</head>

<body>
  <div class="container">
    <div class="logo">
      <img src="https://i.ibb.co/cKHDzHZ6/7992089.png" alt="Access Denied Logo">
    </div>

    <h1>Access Denied</h1>

    <p><b>Thank you for your understanding during this time. Unfortunately, the Company Web firewall policy is currently restricting access to the URL or application you are trying to reach. If you believe this is a mistake, please contact the administrator or try again later.</b></p>

    <div class="contact-info">
      <p>
        For assistance, please reach out to
        <a href="mailto:support@domain.lk" class="link">support@domain.lk</a>
        or Call
        <span class="highlight">0112xxxxxx</span>
      </p>
    </div>

    <table>
      <tbody>
        <tr>
          <td>Category</td>
          <td>%%CATEGORY%%</td>
        </tr>
        <tr>
          <td>URL</td>
          <td>%%PROTOCOL%%://%%URL%%</td>
        </tr>
      </tbody>
    </table>

    <p>
      To have the rating of this web page re-evaluated,
      <a href="%%FTGD_RE_EVAL%%" class="link">please click here</a>.
    </p>

    <p>%%OVERRIDE%%</p>
  </div>
</body>

</html>
``` 
