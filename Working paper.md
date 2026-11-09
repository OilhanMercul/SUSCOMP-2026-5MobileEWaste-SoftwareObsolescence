# Project Working Paper: Software Obsolescence and Frugal Alternatives

---

## 1. Identify the Main Tasks

### 1.1 Software Limitations

Based on the literature review, software obsolescence on aging mobile devices typically stems from a cascade of technical and vendor-driven constraints:

* **Application deprecation:** Applications become non-functional when backward compatibility for older API levels or security protocols is dropped.
* **Storage constraints (Applications):** Applications fail to update or install due to insufficient onboard flash memory.
* **OS version incompatibility:** Applications require newer operating system releases than the device supports.
* **Storage constraints (OS):** System updates cannot be applied due to the growing storage footprint of modern OS builds.
* **End-of-Life (EOL) vendor abandonment:** The manufacturer stops providing firmware updates, security patches, and driver support.

#### Underlying Drivers of Software Limitations

1. **Lack of Upstreaming and Mainlining:**  
   Software and hardware vendors frequently build on vendor-specific forks of open-source components (e.g., the Android kernel and proprietary Board Support Packages / blobs) without contributing code back upstream. Over time, these vendor forks diverge significantly from the mainline branch. Once the vendor ends official support, community-driven maintainers (e.g., custom ROM projects) face an exponential maintenance burden, making it difficult to keep aging chipsets secure and functional.

2. **Economic Incentives and Business Models:**  
   Hardware manufacturers prioritize selling new models rather than allocating engineering resources to backport security patches or optimize newer OS builds for legacy hardware. Long-term maintenance generates little direct revenue, accelerating artificial or planned obsolescence.

3. **Software Bloat and Absence of Graceful Degradation:**  
   Iterative updates often introduce non-essential features, heavier tracking libraries, and unoptimized runtimes, driving up memory (RAM) and storage consumption. Most modern applications lack a *degraded mode*—they fail to provide a lightweight, core-only fallback for constrained hardware, rendering the entire service unusable over minor, unneeded feature additions.

---

### 1.2 Common Tasks and Friction Points on Aging Devices

Drawing from empirical findings in the literature (e.g., *Mosesso et al., 2023, "Obsolescence Paths: Living with Aging Devices"*), several critical use cases and operational failures force users to replace otherwise operational devices:

#### Critical Application Barriers
* **Instant Messaging & VoIP (e.g., WhatsApp, Signal):** Dropped support prevents essential daily communication with family, work, and community.
* **Banking and Payment Apps:** Strict OS integrity and security requirements lock out older OS versions, barring access to financial services.
* **Navigation & Maps:** Core navigation tools become sluggish or drop support, hindering transit and travel.
* **Social Media & Communication Platforms:** Heavy resource footprints cause severe lag or crashes.
* **Media & Streaming Services:** Inability to decode formats or satisfy DRM updates prevents music and video playback.
* **System Utilities & Workflows:** Downloading email attachments, handling notifications reliably, and viewing or editing documents become erratic.

#### System and Hardware Friction Points
In addition to application dropouts, aging devices suffer from systemic degradations:
* **Storage Saturation:** Cache accumulation and growing system partitions trigger continuous low-storage warnings and block critical operations.
* **Performance Throttling & Latency:** High CPU/RAM load causes severe UI stutter, input lag, and unresponsive applications.
* **Battery Degradation & Unexpected Shutdowns:** Voltage drops under high load cause sudden restarts even with reported charge remaining.

#### Target Scope: Core 5 Daily Tasks
To evaluate software alternatives effectively, we focus on the five most critical, high-impact tasks required for everyday digital inclusion:
1. **Messaging and Calling:** Reliable text, voice, and attachment exchange.
2. **Maps and Navigation:** Turn-by-turn routing, transit lookup, and offline mapping.
3. **Internet Browsing:** Secure, lightweight access to web services and information.
4. **Photo and Video Capture:** Camera operation, media storage, and quick previews.
5. **Document Editing & Viewing:** Reading and basic editing of PDFs, spreadsheets, and text files.

---

## 2. Test Mainstream Software and Lightweight Alternatives

### 2.1 Build the Testing Framework and Test Mainstream Software
* Define standardized testing protocols and user scenarios covering the five core tasks.
* Benchmark baseline mainstream applications on legacy hardware (resource utilization: RAM, CPU, storage footprint, and subjective responsiveness/UX latency).

### 2.2 Build the Installation & Testing Framework for Alternative Software
* Identify lightweight, privacy-respecting, and open-source alternatives (e.g., F-Droid catalog, Progressive Web Apps / PWAs, lightweight browsers, and micro-clients).
* Establish repeatable deployment and testing procedures on the target testbed.
* Evaluate alternative solutions against the same performance and usability benchmarks.

---

## 3. Synthesize the Results

* Construct a comparative sustainability and usability matrix contrasting mainstream apps with frugal alternatives.
* Identify trade-offs in functionality, security, user convenience, and hardware resource efficiency.

---

## 4. Calculate the CO2 Impact Reduction

* Quantify the environmental benefits of extending device lifespan (e.g., extending usage from 2–3 years to 5+ years).
* Contrast the avoided embodied carbon footprint (manufacturing, extraction, transport) against running lighter, optimized workloads on existing hardware.
