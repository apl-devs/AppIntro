# ⚠️ Security Notice

This repository and its associated namespace have been claimed as part of a security research project demonstrating **Supply Chain** impact using reborn namespaces in JitPack coordinates.

**This is a benign placeholder. No malicious code is being distributed or published from this repository.**

## 📖 The Research

To understand how this namespace was taken over, the implications for the software supply chain, and how to mitigate this type of vulnerability, please read our full disclosure:

🔗 **[Supply Chain Necromancy: Reborn namespaces in JitPack coordinates](https://labs.itresit.es/2026/02/18/supply-chain-necromancy-reborn-namespaces-in-jitpack-coordinates/)**

## 🛠️ Action Required

If you are looking for the **AppIntro** library, the original project was moved. You must update your build scripts and dependencies to point to the official, actively maintained repository:

👉 **[https://github.com/AppIntro/AppIntro](https://github.com/AppIntro/AppIntro)**

Continuing to use the old coordinates (`apl-devs/AppIntro`) exposes your software supply chain to hijacking risks.

### Recommended Fix

Update your `build.gradle` file:

```gradle
// DELETE THIS LINE:
// implementation 'com.github.apl-devs:appintro:x.y.z'

// REPLACE WITH:
implementation 'com.github.AppIntro:AppIntro:x.y.z'
```
---

*This proof of concept was conducted by LABS @ ITRES for educational and responsible disclosure purposes.*
