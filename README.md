/* ------------------------------------------------
   Instagram Login Page - Main Stylesheet
   Inspired by original design, fully responsive
--------------------------------------------------- */

/* ----- Base &  life reset ----- */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
}

body {
  background-color: #fafafa;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  padding: 12px;
}

/* ----- main container (flex row) ----- */
.container {
  max-width: 935px;
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  gap: 32px;
  margin: 24px auto;
}

/* ----- left side: phone mockup (hidden on small screens) ----- */
.phone-mock {
  display: none;
  flex: 1;
  min-width: 380px;
  justify-content: flex-end;
}

@media (min-width: 876px) {
  .phone-mock {
    display: flex;
  }
}

.phone-frame {
  background: #ffffff;
  border: 1px solid #dbdbdb;
  border-radius: 42px;
  padding: 12px;
  box-shadow: 0 0 20px rgba(0,0,0,0.03);
  width: 380px;
  height: 586px;
  position: relative;
}

.phone-screen {
  background: linear-gradient(145deg, #f3e7e9 0%, #e3d2e4 40%, #c7d4e8 100%);
  width: 100%;
  height: 100%;
  border-radius: 32px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: rgba(0,0,0,0.2);
  font-size: 14px;
  overflow: hidden;
  position: relative;
}

/* decorative app icons inside phone */
.phone-screen .mock-stories {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  padding: 20px;
  justify-content: center;
}

.mock-stories span {
  background: rgba(255,255,255,0.65);
  backdrop-filter: blur(4px);
  width: 60px;
  height: 60px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 4px 12px rgba(0,0,0,0.05);
  font-size: 28px;
  color: #262626;
}

/* ----- right side: login card + footer ----- */
.login-section {
  flex: 1;
  min-width: 350px;
  max-width: 400px;
}

/* main white card */
.login-card {
  background: #ffffff;
  border: 1px solid #dbdbdb;
  border-radius: 1px;
  padding: 40px 40px 36px;
  margin-bottom: 10px;
}

/* instagram wordmark (uses google font as fallback) */
.logo {
  font-family: 'Grand Hotel', cursive, 'Segoe UI';
  font-size: 50px;
  font-weight: 400;
  text-align: center;
  margin-bottom: 24px;
  letter-spacing: -0.5px;
  color: #262626;
}

/* ----- login form ----- */
.login-form {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.input-field {
  background: #fafafa;
  border: 1px solid #dbdbdb;
  border-radius: 3px;
  padding: 9px 0 7px 8px;
  font-size: 12px;
  outline: none;
  transition: border-color 0.1s;
}

.input-field:focus {
  border-color: #a8a8a8;
}

.input-field::placeholder {
  color: #8e8e8e;
}

.login-btn {
  background-color: #0095f6;
  border: none;
  border-radius: 8px;
  padding: 7px 16px;
  font-weight: 600;
  font-size: 14px;
  color: white;
  margin-top: 12px;
  cursor: pointer;
  transition: background 0.2s;
}

.login-btn:hover {
  background-color: #1877f2;
}

.login-btn:active {
  opacity: 0.7;
}

/* ----- divider with OR ----- */
.divider {
  display: flex;
  align-items: center;
  margin: 20px 0 18px;
  color: #8e8e8e;
  font-size: 13px;
  font-weight: 600;
  gap: 18px;
}

.divider-line {
  flex: 1;
  height: 1px;
  background: #dbdbdb;
}

/* ----- facebook login button ----- */
.fb-login {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: none;
  border: none;
  color: #385185;
  font-weight: 600;
  font-size: 14px;
  cursor: pointer;
  margin-bottom: 12px;
  width: 100%;
  padding: 6px;
}

.fb-login i {
  font-size: 18px;
}

.forgot-password {
  display: block;
  text-align: center;
  color: #00376b;
  font-size: 12px;
  text-decoration: none;
  margin-top: 16px;
}

.forgot-password:hover {
  text-decoration: underline;
}

/* ----- sign up card (second box) ----- */
.signup-card {
  background: #ffffff;
  border: 1px solid #dbdbdb;
  padding: 22px 40px;
  text-align: center;
  font-size: 14px;
  margin-bottom: 20px;
}

.signup-card a {
  color: #0095f6;
  font-weight: 600;
  text-decoration: none;
}

.signup-card a:hover {
  text-decoration: underline;
}

/* ----- app download section ----- */
.app-links {
  text-align: center;
  margin: 16px 0 40px;
}

.app-links p {
  font-size: 14px;
  color: #262626;
  margin-bottom: 16px;
}

.store-badges {
  display: flex;
  gap: 8px;
  justify-content: center;
}

/* simple simulated badges (instead of images) */
.badge {
  background: #262626;
  color: white;
  border-radius: 6px;
  padding: 6px 12px;
  font-size: 11px;
  font-weight: 600;
  display: inline-flex;
  align-items: center;
  gap: 5px;
  opacity: 0.9;
}

.badge i {
  font-size: 16px;
}

/* ----- footer (meta links) ----- */
.footer {
  max-width: 935px;
  width: 100%;
  margin-top: 24px;
  text-align: center;
  color: #8e8e8e;
  font-size: 12px;
}

.footer-links {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 8px 16px;
  margin-bottom: 16px;
}

.footer-links a {
  color: #8e8e8e;
  text-decoration: none;
  font-size: 12px;
}

.footer-links a:hover {
  text-decoration: underline;
}

.copyright {
  margin-top: 8px;
}

.footer-sep {
  color: #8e8e8e;
}

/* small note (demo disclaimer) */
.demo-note {
  font-size: 10px;
  color: #999;
  margin-top: 8px;
  text-align: center;
  width: 100%;
}
