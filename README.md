```
# Shithub — The Chaos Archive

> Songs that hit harder than a kernel panic
> One song away from total system failure

## ⚠️ BIG WARNING
- This site is made for Linux users only
- Windows browsers get automatically kicked out
- The kernel panic commands are EXTREMELY DANGEROUS — SAVE ALL WORK, use a VM or test device ONLY!

## 🧠 Full Magic SysRq Kernel Panic Tutorial

### 1. Check current SysRq status
```bash
cat /proc/sys/kernel/sysrq
```

- `0` = fully disabled
- `16` = limited, cannot trigger panic
- `1` = FULLY UNLOCKED, ready to use

### 2. Temporarily enable full SysRq (resets after reboot)

```
su
echo 1 > /proc/sys/kernel/sysrq
```

### 3. Trigger kernel panic

```
echo c > /proc/sysrq-trigger
```

Your system will panic, freeze and restart instantly.

### 4. Make SysRq=1 permanent (optional)

```
echo "kernel.sysrq = 1" >> /etc/sysctl.conf
sysctl -p
```

## 🚀 How to Run Shithub

### Option A: Open directly in browser

👉 **Visit: [https://shithub.vercel.app/](https://shithub.vercel.app/)**

### Option B: Download with curl and open locally

```
# Download the full page
curl -o shithub.html https://shithub.vercel.app/

# Open it in your default browser
xdg-open shithub.html
```

### Option C: Just view it directly in your browser

No download needed — just open: **[https://shithub.vercel.app/](https://shithub.vercel.app/)** 🎉

---

🐧 **Welcome to the chaos — Linux only!!!** 🐧

```

Everything's clean, all steps inside the README, and your official link is ready bro!!! 😎💚🚀
```
