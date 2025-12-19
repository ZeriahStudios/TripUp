---
layout: default
title: Submit
permalink: /submit/
---

## Submit a Trip Up

Share a mistake so others don’t have to repeat it.

<form action="/submit" method="POST">

  <label>
    Area
    <select name="area" required>
      <option value="Travel">Travel</option>
      <option value="Parenting">Parenting</option>
      <option value="Work">Work</option>
      <option value="Life">Life</option>
      <option value="Other">Other</option>
    </select>
  </label>

  <br><br>

  <label>
    Category
    <input type="text" name="category" placeholder="e.g. Assumption, Oversight" required>
  </label>

  <br><br>

  <label>
    Contributor (optional)
    <input type="text" name="contributor" placeholder="Anonymous">
  </label>

  <br><br>

  <label>
    What happened?
    <textarea name="content" rows="6" required
      placeholder="Describe the mistake clearly (at least 20 characters)"></textarea>
  </label>

  <br><br>

  <label>
    Reflection (optional)
    <textarea name="reflection" rows="4"
      placeholder="What would you do differently next time?"></textarea>
  </label>

  <br><br>

  <!-- Cloudflare Turnstile -->
  
  <div class="cf-turnstile"
       data-sitekey="0x4AAAAAACHlNYb2XdMxSePD"></div>

  <br><br>

  <button type="submit">Submit Trip Up</button>

</form>

<p style="opacity:0.7; margin-top:1em;">
Submissions are reviewed before appearing publicly.
</p>
