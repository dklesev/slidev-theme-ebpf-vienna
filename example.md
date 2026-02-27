---
theme: ./
date: dd.mm.yyyy
addons:
  - slidev-component-spotlight
  - slidev-addon-qrcode
---

# Slidev Theme

optional topic subtitle

---
layout: lead
---

<div class="lead-logo">
  <img src="/ebpf-logo.png" class="logo-light" />
  <img src="/ebpf-logo-dark.png" class="logo-dark" />
</div>

(recap)

<style>
.lead-logo {
  display: flex;
  justify-content: center;
}
.lead-logo img {
  width: 7.5em;
  position: relative;
  top: -1em;
}
p {
  position: relative;
  top: -2em;
}
</style>

---
layout: image
image: https://www.brendangregg.com/eBPF/linux_ebpf_support.png
backgroundSize: 53%
---

# eBPF

<span class="see">See: https://www.brendangregg.com/ebpf.html</span>

---
layout: lead
---

# Hello eBPF

---

# Hello eBPF | Example

*(simple ebpf program)*

<<< @/snippets/example.c c {|4|4,7|}{lines: true}

---
layout: lead
---

# DEMO

---
layout: vhs
---

<SlidevVideo v-click autoplay controls>
  <source src="/demo.mp4" type="video/mp4" />
  <p>
    Your browser does not support videos. You may download it
    <a href="/demo.mp4">here</a>.
  </p>
</SlidevVideo>

---
layout: empty
---

---
layout: center
class: "text-center"
---

# Learn More

[eBPF](https://ebpf.io) / [meetup](https://www.meetup.com/ebpf-vienna/)

---
layout: empty
---

<div class="flex flex-col items-center">
<br><br><br>

<div class="logo-light">
<QRCode
    :width="300"
    :height="300"
    type="svg"
    data="https://www.meetup.com/ebpf-vienna/"
    :margin="10"
    :imageOptions="{ margin: 10 }"
    :dotsOptions="{ type: 'extra-rounded', color: '#00AEEF' }"
    :cornersSquareOptions="{ type: 'dot', color: '#000000' }"
    :cornersDotOptions="{ type: 'dot', color: '#000000' }"
    :backgroundOptions="{ color: 'transparent' }"
    image="/ebpf-icon.png"
/>
</div>

<div class="logo-dark">
<QRCode
    :width="300"
    :height="300"
    type="svg"
    data="https://www.meetup.com/ebpf-vienna/"
    :margin="10"
    :imageOptions="{ margin: 10 }"
    :dotsOptions="{ type: 'extra-rounded', color: '#71d9ffff' }"
    :cornersSquareOptions="{ type: 'dot', color: '#ffffff' }"
    :cornersDotOptions="{ type: 'dot', color: '#ffffff' }"
    :backgroundOptions="{ color: 'transparent' }"
    image="/ebpf-icon-dark.png"
/>
</div>

</div>