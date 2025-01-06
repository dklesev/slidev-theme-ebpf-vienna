---
theme: ./
date: 05.03.2025
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

<see>See: https://www.brendangregg.com/ebpf.html</see>

---
layout: lead
---

# Hello eBPF

---

# Hello eBPF

*(simple ebpf program)*

```c
#include <vmlinux.h>
#include <bpf/bpf_helpers.h>

SEC("tracepoint/syscalls/sys_enter_execve")
int bpf_prog(void *ctx)
{
  bpf_printk("Hello eBPF!");
  return 0;
};

char LICENSE[] SEC("license") = "GPL";
```

---
layout: center
class: "text-center"
---

# Learn More

[eBPF](https://ebpf.io) / [meetup](https://www.meetup.com/ebpf-vienna/)
