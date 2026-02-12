<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>
      Authentication
    </title>
    <style>
      * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
      }
      body {
        min-height: 100vh;
        font-family: Arial, sans-serif;
        background: linear-gradient(to right, #0a0f1f, #141a33);
        color: #e0e6f0;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        padding: 20px;
      }
      .login-container {
        background: #12182b;
        padding: 40px 30px;
        border-radius: 15px;
        box-shadow: 0 8px 30px rgba(0, 0, 0, 0.6);
        width: 100%;
        max-width: 400px;
        animation: fadeIn 0.8s ease-in-out;
      }
      /* FortiGate Logo */
      .logo {
        height: 120px;
        margin-bottom: 20px;
        background: url(%%IMAGE:block_logo%%) no-repeat center center;
        background-size: contain;
      }
      h2 {
        text-align: center;
        margin-bottom: 10px;
        color: #ff4d4d;
      }
      .subtext {
        text-align: center;
        font-size: 14px;
        color: #aab4d6;
        margin-bottom: 15px;
      }
      .validation-msg {
        background-color: #161d35;
        border-left: 4px solid #ff4d4d;
        padding: 12px 16px;
        margin-bottom: 20px;
        color: #cbd3e6;
        font-size: 14px;
        border-radius: 6px;
        text-align: center;
      }
      .input-group {
        margin-bottom: 15px;
      }
      label {
        display: block;
        margin-bottom: 6px;
        font-size: 14px;
        color: #cbd3e6;
      }
      input[type="text"],
      input[type="password"] {
        width: 100%;
        padding: 10px;
        background-color: #161d35;
        border: 1px solid #2a3355;
        border-radius: 6px;
        color: #e0e6f0;
      }
      input:focus {
        outline: none;
        border-color: #6ea8ff;
        box-shadow: 0 0 6px rgba(110,168,255,0.5);
      }
      .btn {
        width: 100%;
        padding: 12px;
        background-color: #ff4d4d;
        color: #fff;
        border: none;
        border-radius: 6px;
        font-weight: bold;
        cursor: pointer;
        margin-top: 10px;
        transition: 0.2s ease-in-out;
      }
      .btn:hover {
        background-color: #ff6666;
        transform: translateY(-1px);
      }
      .footer-msg {
        margin-top: 30px;
        text-align: center;
        font-size: 13px;
        color: #aab4d6;
        max-width: 500px;
        line-height: 1.6;
      }
      .footer-msg .highlight {
        color: #6ea8ff;
        font-weight: bold;
      }
      .footer-msg .link {
        color: #6ea8ff;
        text-decoration: none;
        font-weight: bold;
      }
      .footer-msg .link:hover {
        text-decoration: underline;
        color: #9ec5ff;
      }
      @keyframes fadeIn {
        from {
          opacity: 0;
          transform: translateY(8px);
        }
        to {
          opacity: 1;
          transform: translateY(0);
        }
      }
    </style>
  </head>
  <body>
    <div class="login-container">
      <div class="logo">
      </div>
      <h2>
        Authentication Required
      </h2>
      <p class="subtext">
        Please enter your credentials to continue.
      </p>
      <div class="validation-msg">
        We need to validate your user login.
        <br>
        Please enter your login credentials to proceed.
      </div>
      <form action="%%AUTH_POST_URL%%" method="post">
        <input type="hidden" name="%%REDIRID%%" value="%%PROTURI%%">
        <input type="hidden" name="%%MAGICID%%" value="%%MAGICVAL%%">
        <input type="hidden" name="%%METHODID%%" value="%%METHODVAL%%">
        <div class="input-group">
          <label for="ft_un">
            Username
          </label>
          <input name="%%USERNAMEID%%" id="ft_un" type="text" required>
        </div>
        <div class="input-group">
          <label for="ft_pd">
            Password
          </label>
          <input name="%%PASSWORDID%%" id="ft_pd" type="password" required>
        </div>
        <button class="btn" type="submit">
          Continue
        </button>
      </form>
    </div>
    <div class="footer-msg">
      For further issues or complaints, contact
      <span class="highlight">
        Data Center
      </span>
      <br>
      Email:
      <a href="mailto:user@domain.lk" class="link">
        user@domain.lk
      </a>
      |
      TP:
      <span class="highlight">
        xxx-xxxxxx46
      </span>
    </div>
  </body>
</html>
