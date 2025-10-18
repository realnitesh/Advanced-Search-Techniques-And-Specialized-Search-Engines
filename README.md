# 🔍 Advanced Search Techniques And Specialized Search Engines

This guide helps you **search smarter** on the internet using **Google Search Operators** and explore **specialized search engines** like **Shodan**, **Censys**, **VirusTotal**, and **Have I Been Pwned** — all useful for **researchers, cybersecurity learners, and developers**.

---

## 🧠 1. Google Search Operators

Google supports **advanced search operators** that help refine and narrow down search results.
You can combine multiple operators for powerful queries.

| Operator    | Description                            | Example                                               |
| ----------- | -------------------------------------- | ----------------------------------------------------- |
| `site:`     | Search within a specific website       | `site:wikipedia.org AI` → Finds AI pages on Wikipedia |
| `filetype:` | Find specific file types               | `filetype:pdf ethical hacking`                        |
| `intitle:`  | Find pages with a word in the title    | `intitle:"login page"`                                |
| `inurl:`    | Find pages with keywords in the URL    | `inurl:admin`                                         |
| `cache:`    | View Google’s cached version of a page | `cache:example.com`                                   |
| `related:`  | Find sites related to a domain         | `related:youtube.com`                                 |
| `" "`       | Search for an exact phrase             | `"how to secure linux server"`                        |
| `-`         | Exclude a term                         | `python -snake`                                       |
| `OR`        | Search for either term                 | `devops OR cloud`                                     |
| `*`         | Wildcard for unknown terms             | `"best * tools"`                                      |
| `define:`   | Get a quick definition                 | `define:cybersecurity`                                |

### 💡 Example: Combine Operators

```bash
site:github.com filetype:py "password" inurl:config
```

This finds **Python configuration files** on GitHub that may contain the word *password* — often used in **security research** or **open-source analysis**.

---

## 🌐 2. Specialized Search Engines

Beyond Google, there are **search engines designed for cybersecurity and internet research**.
Let’s explore the most popular ones 👇

---

### 🛰️ **Shodan**

**Website:** [https://www.shodan.io/](https://www.shodan.io/)

Shodan is a **search engine for internet-connected devices** (IoT, routers, cameras, servers, etc.).
It helps you find **which devices are publicly accessible** and what software they run.

#### 🔹 Example Searches:

| Query                 | Description                  |
| --------------------- | ---------------------------- |
| `apache country:"IN"` | Find Apache servers in India |
| `port:22`             | Devices with SSH open        |
| `title:"webcamXP"`    | Find public webcams          |
| `org:"Amazon.com"`    | Devices hosted by Amazon     |

⚠️ **Use ethically** — for research, vulnerability testing (with permission), and learning.

---

### 🔎 **Censys**

**Website:** [https://search.censys.io/](https://search.censys.io/)

Censys scans the **entire internet** and indexes hosts, certificates, and services.
It’s used to analyze **SSL/TLS certificates**, open ports, and exposed devices.

#### 🔹 Example Searches:

| Query                                                                  | Description                             |
| ---------------------------------------------------------------------- | --------------------------------------- |
| `services.service_name:HTTP`                                           | Show all HTTP servers                   |
| `location.country:India`                                               | Hosts located in India                  |
| `services.tls.certificates.leaf_data.subject.common_name:*.google.com` | Find Google subdomains via certificates |

---

### 🦠 **VirusTotal**

**Website:** [https://www.virustotal.com/](https://www.virustotal.com/)

VirusTotal is a free service to **analyze files and URLs for malware** using multiple antivirus engines.

#### 🔹 Uses:

* Upload suspicious files or links
* Check if a URL is flagged as malicious
* Search by hash (MD5, SHA256)

#### 🔹 Example:

```
https://www.virustotal.com/gui/file/<SHA256_HASH>
```

Use it for **malware investigation, threat intelligence**, and **file reputation checks**.

---

### 🔐 **Have I Been Pwned (HIBP)**

**Website:** [https://haveibeenpwned.com/](https://haveibeenpwned.com/)

HIBP lets you check if your **email or password was exposed in a data breach**.

#### 🔹 How to Use:

1. Visit [haveibeenpwned.com](https://haveibeenpwned.com/)
2. Enter your **email**
3. It will show whether it appeared in any known data breach

#### 🔹 API Example:

```bash
https://haveibeenpwned.com/api/v3/breachedaccount/<email>
```

Great for **personal security awareness** and **credential monitoring**.

---

## ⚙️ Summary Table

| Tool                  | Focus Area             | Common Use                        |
| --------------------- | ---------------------- | --------------------------------- |
| **Google Operators**  | Smart web searches     | Precise data & research           |
| **Shodan**            | IoT / Internet devices | Find exposed servers & cameras    |
| **Censys**            | Network scanning       | SSL, IP, domain security research |
| **VirusTotal**        | File & URL scanning    | Malware detection                 |
| **Have I Been Pwned** | Breach monitoring      | Check compromised accounts        |

---

## ⚠️ Disclaimer

These tools are intended for **educational and ethical research** only.
**Never use them to access or exploit systems without permission.**
Always follow **cybersecurity laws and responsible disclosure** practices.

---

## 🧰 Resources & Links

* [Google Advanced Search](https://support.google.com/websearch/answer/2466433)
* [Shodan Documentation](https://developer.shodan.io/)
* [Censys Docs](https://search.censys.io/)
* [VirusTotal API](https://developers.virustotal.com/)
* [Have I Been Pwned API](https://haveibeenpwned.com/API/v3)

---

### ✨ Author

**Created by:** Nitesh Kumar
**Purpose:** To help learners and researchers explore the power of search intelligence easily.

---
