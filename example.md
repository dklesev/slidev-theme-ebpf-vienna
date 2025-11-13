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

![](https://ebpf.foundation/wp-content/uploads/sites/9/2023/03/ebpf_logo_color_on_white-2-300x108.png)

(recap)

<style>
img {
  position: relative;
  width: 7.5em;
  left: 40%;
}
p {
  position: relative;
  bottom: 2em;
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
    image="/ebpf-icon.png"
/>

</div>