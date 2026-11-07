# Software Obsolescence: Analysis and Remediation Strategies

> **Source** : Doctoral thesis — Analysis of the software obsolescence phenomenon and remediation strategies, with focus on **Android** and **Debian**.

---

## Overview

This doctoral thesis analyses the software obsolescence phenomenon and proposes remediation strategies. It focuses on two main software ecosystems — **Android** and **Debian** — examining their development strategies, problems, and solutions.

A key finding on Debian: **software updates do not necessarily imply hardware obsolescence**. Software obsolescence is primarily driven by **economic strategies**.

---

## Key Policy Recommendations

The thesis identifies the following core solutions:

- Updates should **not discard hardware**;
- Updates should **not introduce breaking changes** and should provide **retrocompatibility for long periods** (minimum 10 years);
- If breaking changes are unavoidable, they should be **set aside, discussed, and evaluated** with the affected user and developer communities until a common solution and process are established;
- Require device vendors to **publish update and upgrade plans** for every device, and ensure they are followed;
- Require device vendors, chip and parts manufacturers, and software companies to **liberate all code, schematics, and documentation** related to hardware behavior whenever they stop providing updates, and upon expiration of the warranty and support period;
- **Include mainlining and upstreaming conditionality** into Free and Open Source licenses;
- Require all OS components, firmware, and software in boot sequences to be **maintained for at least 10 years**;
- All OS components, firmware, and software in boot sequences should follow (or define) **open public standards**, to avoid proprietary software lock-ins;
- Consider operating systems, firmware, and software in boot sequences as **public infrastructure, governed as digital commons**.

---

## Chapter Notes

### §1.3.5 & §1.3.6 — Software Obsolescence and Maintenance

The author discusses the concepts of software obsolescence and maintenance, highlighting that most maintenance work consists of **adding new features rather than preserving functionality**:

> *"75% to 80% are related to enhancements rather than corrections."*

He also notes that *"discontinued software support is a replacement reason"*, and argues that libre/community-driven software **"do not have an inbuilt growth compulsion as is usually the case in capitalism and thus better allow for sustainability"**.

Finally, he reframes devices as **"fragile objects, with a constant need for care to remain functional"**.

---

### §2.4.4 — Successes and Limits of Obsolescence Circumvention Strategies

The author examines strategies to circumvent software obsolescence for devices, with notable case studies on **LineageOS** and **Fairphone**, which had to **backport several updates** to keep devices functional.

Key takeaways:
- Backporting is **very difficult** and only a **temporary solution**;
- LineageOS frequently **abandons older devices** over time;

> *"As smartphones get older and new hardware is released, the burden of kernel maintenance grows, while the number of users and maintainers for older devices shrinks, thus decreasing the possibility of sustainably maintaining code."*

---

### §2.5.1 — Updates as a Double-Edged Sword

The author questions updates as a solution to obsolescence. Sometimes updates **cause obsolescence** or become more of a **burden than a solution**.

---

### §2.6 — Android: Conclusion

Android OS versions are built **per device**, with a short lifespan. Phone manufacturers do not update them for long. Key problems identified:

- Phone vendors **do not contribute to upstreaming**, making maintainability harder;
- Google's strategy of **enforcing its own services and software**, combined with reluctance to upstream from SoC manufacturers and phone vendors, is a major obstacle to long-term maintainability.

---

### §3.4.2 — Debian Kernel Maintenance

Debian maintenance teams are **mainlining the Debian kernel with the upstream Linux kernel**, ensuring it stays up to date for security and other improvements.

---

### §3.6 — Debian: Conclusion

By adopting a solid maintenance strategy, **Debian facilitates the maintenance of other hardware and software ecosystems**.

---

### §5.1.1 — Android Kernel Divergence

> *"The lack of updates appears, in particular, at the kernel level, i.e., at the core of Android builds, as the code from phone vendors and system on chip manufacturers increasingly diverges from the original Linux kernel code."*

The author also discusses the various problems that **Google's near-monopoly** causes for the maintainability of Android devices.

---

### §5.1.2 — (Additional Notes)

This section does not add significantly new content relative to the topics covered above.
