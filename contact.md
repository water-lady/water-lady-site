---
layout: default
title: Contact
---

<p class="contact-intro">If you would like to connect, please share your info below and I will get back to you as soon as possible.</p>

<form action="https://formspree.io/f/mzzjgdok" method="POST" class="contact-form">
  <div class="form-group">
    <label for="name">Name *</label>
    <input type="text" name="name" id="name" required>
  </div>
  
  <div class="form-group">
    <label for="email">Email *</label>
    <input type="email" name="_replyto" id="email" required>
  </div>
  
  <div class="form-group">
    <label for="company">Company/Organization</label>
    <input type="text" name="company" id="company">
  </div>
  
  <div class="form-group">
    <label for="phone">Phone Number</label>
    <input type="tel" name="phone" id="phone">
  </div>
  
  <div class="form-group">
    <label for="subject">Subject *</label>
    <select name="subject" id="subject" required>
      <option value="">Select a topic...</option>
      <option value="FEED Study">FEED Study</option>
      <option value="Process Design">Process Design</option>
      <option value="QAQC Review">QAQC Review</option>
      <option value="General Inquiry">General Inquiry</option>
      <option value="Other">Other</option>
    </select>
  </div>
  
  <div class="form-group">
    <label for="message">Message *</label>
    <textarea name="message" id="message" rows="6" required></textarea>
  </div>
  
  <!-- Hidden field for spam protection -->
  <input type="text" name="_gotcha" style="display:none">
  
  <!-- Success message redirect (optional) -->
  <input type="hidden" name="_next" value="/contact-success.html">
  
  <button type="submit" class="btn-submit">Send Message</button>
</form>

<style>
.contact-intro {
  max-width: 600px;
  margin: 20px auto 40px auto;
  text-align: center;
  color: #6c757d;
  font-size: 1.1em;
  line-height: 1.6;
}

.contact-form {
  max-width: 600px;
  margin: 40px auto;
  padding: 40px;
  background: white;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.08);
}

.form-group {
  margin-bottom: 25px;
}

.form-group label {
  display: block;
  margin-bottom: 8px;
  color: #2b2d2f;
  font-weight: 500;
  font-size: 0.95em;
}

.form-group input,
.form-group select,
.form-group textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ddd;
  border-radius: 4px;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  transition: border-color 0.3s;
  box-sizing: border-box;
}

.form-group input:focus,
.form-group select:focus,
.form-group textarea:focus {
  outline: none;
  border-color: #2c5f7a;
  box-shadow: 0 0 0 3px rgba(44, 95, 122, 0.1);
}

.form-group select {
  cursor: pointer;
  background: white;
}

.form-group textarea {
  resize: vertical;
  min-height: 120px;
}

.btn-submit {
  background: #2c5f7a;
  color: white;
  padding: 14px 40px;
  border: none;
  border-radius: 5px;
  font-weight: 600;
  font-size: 16px;
  cursor: pointer;
  transition: all 0.3s;
  width: 100%;
}

.btn-submit:hover {
  background: #3d4a54;
  transform: translateY(-2px);
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
}

.btn-submit:active {
  transform: translateY(0);
}

@media (max-width: 768px) {
  .contact-form {
    padding: 30px 20px;
    margin: 20px;
  }
}
</style>