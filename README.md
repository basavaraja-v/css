1. Recently fine-tuned chatGPT on custom data [Check here](https://colab.research.google.com/drive/1KTKJ5-95bhf0zyRJwnKBYzHkTVV-i9rR#scrollTo=0deDr8vKIDFy)
2. Below are the smaple chatGPT prompts used to design sign with google
- Prompt: generate professional looking login ui/ux, sign with google and write index.html

- ChatGPT: Here's an example of a professional-looking login UI/UX design with sign-in with Google option:

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Login Page</title>
    <style>
      /* Add styles for the page */
      body {
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: #F2F2F2;
        height: 100vh;
      }
      
      form {
        background-color: #FFFFFF;
        box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        padding: 40px;
        border-radius: 10px;
        width: 400px;
        display: flex;
        flex-direction: column;
        align-items: center;
      }
      
      h1 {
        font-size: 36px;
        font-weight: bold;
        margin-bottom: 20px;
        text-align: center;
      }
      
      input[type="email"], input[type="password"] {
        width: 100%;
        padding: 10px;
        margin-bottom: 20px;
        border: none;
        border-radius: 5px;
        font-size: 18px;
      }
      
      input[type="submit"] {
        width: 100%;
        padding: 10px;
        background-color: #4285F4;
        color: #FFFFFF;
        border: none;
        border-radius: 5px;
        font-size: 18px;
        cursor: pointer;
      }
      
      .google-sign-in {
        width: 100%;
        padding: 10px;
        background-color: #FFFFFF;
        border: 1px solid #000000;
        border-radius: 5px;
        font-size: 18px;
        cursor: pointer;
        display: flex;
        align-items: center;
        margin-top: 20px;
      }
      
      .google-icon {
        width: 20px;
        height: 20px;
        margin-right: 10px;
      }
    </style>
  </head>
  <body>
    <form>
      <h1>Login</h1>
      <input type="email" placeholder="Email">
      <input type="password" placeholder="Password">
      <input type="submit" value="Login">
      <div class="google-sign-in">
        <img class="google-icon" src="https://upload.wikimedia.org/wikipedia/commons/5/53/Google_%22G%22_Logo.svg">
        Sign in with Google
      </div>
    </form>
  </body>
</html>
```

Note: This is just an example, you may need to add your own styling and functionality to the code to make it fit your specific needs.

- Prompt: update only css to display Sign in with Google in center

- ChatGPT: You can update the CSS to display the "Sign in with Google" text in the center of the button as follows:

```
.google-sign-in {
  width: 100%;
  padding: 10px;
  background-color: #FFFFFF;
  border: 1px solid #000000;
  border-radius: 5px;
  font-size: 18px;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 20px;
}
```

- Prompt: match the width of google sign in button with submit button

- ChatGPT: You can match the width of the "Sign in with Google" button with the submit button by giving both buttons the same width, for example:

```
input[type="submit"], .google-sign-in {
  width: 100%;
  padding: 10px;
}

input[type="submit"] {
  background-color: #4285F4;
  color: #FFFFFF;
  border: none;
  border-radius: 5px;
  font-size: 18px;
  cursor: pointer;
}

.google-sign-in {
  background-color: #FFFFFF;
  border: 1px solid #000000;
  border-radius: 5px;
  font-size: 18px;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 20px;
}
```
By giving both buttons the same width property, they will have the same width.

- Prompt: integrate in index.html

- ChatGPT:
Here's an updated version of the index.html file that includes the integration of the "Sign in with Google" button:

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Login Page</title>
    <style>
      /* Add styles for the page */
      body {
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: #F2F2F2;
        height: 100vh;
      }
      
      form {
        background-color: #FFFFFF;
        box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        padding: 40px;
        border-radius: 10px;
        width: 400px;
        display: flex;
        flex-direction: column;
        align-items: center;
      }
      
      h1 {
        font-size: 36px;
        font-weight: bold;
        margin-bottom: 20px;
        text-align: center;
      }
      
      input[type="email"], input[type="password"] {
        width: 100%;
        padding: 10px;
        margin-bottom: 20px;
        border: none;
        border-radius: 5px;
        font-size: 18px;
      }
      
      input[type="submit"], .google-sign-in {
        width: 100%;
        padding: 10px;
      }
      
      input[type="submit"] {
        background-color: #4285F4;
        color: #FFFFFF;
        border: none;
        border-radius: 5px;
        font-size: 18px;
        cursor: pointer;
      }
      
      .google-sign-in {
        background-color: #FFFFFF;
        border: 1px solid #000000;
        border-radius: 5px;
        font-size: 18px;
        cursor: pointer;
        display: flex;
        align-items: center;
        justify-content: center;
        margin-top: 20px;
      }
      
      .google-icon {
        width: 20px;
        height: 20px;
        margin-right: 10px;
      }
    </style>
  </head>
  <body>
    <form>
      <h1>Login</h1>
      <input type="email" placeholder="Email">
      <input type="password" placeholder="Password">
      <input type="submit" value="Login">
      <div class="google-sign-in">
        <img class="google-icon" src="https://upload.wikimedia.org/wikipedia/commons/5/53/Google_%22G%22_Logo.svg">
        Sign in with Google
      </div>
    </form>
  </body>
</html>
```
