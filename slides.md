---
# try also 'default' to start simple
theme: seriph
background: https://fqme.qc.ca/wp-content/uploads/2018/09/DJI_0137.jpg
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Lac long challenge
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS
css: unocss
---

# The Lac Long Challenge


---
layout: two-cols
---
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d59082.044452870956!2d-72.12980152904402!3d46.80516983353783!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4cc70d86b268e54b%3A0xb51c1a8e86cd5aca!2sLac%20Long%20-%20Site%20d&#39;escalade%20de%20la%20FQME!5e0!3m2!1sen!2sca!4v1666126910612!5m2!1sen!2sca" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>

---
layout:image
---
##  Francis, Louit, Alex, Me
![climbers](/lac-long-challenge-climbers.JPG)

---
layout: quote
---

# The Challenge

The first climber to do all the routes that all other climbers have done wins


<div class="flex justify-evenly">

<div class="" v-click>

### Louit
<img src="/louit.png" class="h-20 rounded shadow mr-4"/> 

- Aéro-Tango 
- Anticipation
</div>

<div class="" v-click>

### Me
<img src="/me.jpg" class="h-20 rounded shadow inline-block mr-4" /> 

- Aéro-Tango 
- Postes Canada  
</div>

<div class="" v-click>

### Alex
<img src="/alex.png" class="h-20 rounded shadow inline-block mr-4" /> 

- Le Matelot
- Anticipation
- Atmosphéria
</div>

<div class="" v-click>

### Francis  
<img src="/francis.png" class="h-20 rounded shadow inline-block mr-4" /> 

- Aéro-Tango 
- Postes Canada
- Anticipation
- Le Matelot
- Atmosphéria
</div>

</div>

---
layout:statement
---

I want to easily know which routes I have left to win the challenge

![background](/lac-long-background.JPG)

---
layout: two-cols 
---

# Requirements

- Cheap
- Easy to maintain 
- Write once and forget about it
- Not spend too much time on it
- Easy to deploy
- Fast

::right::

<v-click>

- No database
- No javascript
- Min dependencies

<img src="/aero-tango.jpg" class="h-90 rounded shadow inline-block mr-4" /> 
</v-click>

---
---
# Deploying

- Linode / Digital Ocean: Too expensive
- Render: free tier becomes inactive after 15 min and hard to debug

<v-click>

## Flying with Fly.io <logos-fly-icon class="text-6xl inline-block" /> 

- CLI is awesome `fly launch && fly deploy`
- Docker without docker
- Storage 
- Cheap 
- Control (easy to debug)
</v-click>

---
layout: iframe
url: https://www.mountainproject.com/user/200222284/daniel-rodas-bautista/ticks
---

# Mountain Project 

--- 
layout: iframe-right
url: https://laclong.fly.dev

---
# Putting it all together

[laclong.fly.dev](https://laclong.fly.dev)
- Fetch CSVs daily 
- Simple Go server <logos-gopher class="text-3xl" />
- pico CSS
- Go HTML template
- Deployed to fly.io Toronto <logos-fly-icon class="text-3xl" />





