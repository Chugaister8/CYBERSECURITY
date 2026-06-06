# Підбірка матеріалів для самостійного навчання з кібербезпеки
### На основі CSEC2017 · Загальна кібербезпека · Самостійне навчання

---

> **Як користуватися цією підбіркою.** Матеріали організовано за 8 галузями знань CSEC2017. У кожній галузі є три шари: підручники (теорія), онлайн-курси (структуроване навчання) та практичні інструменти (застосування). Рекомендований порядок: спочатку пройдіть усі основні елементи кожної галузі, потім поглиблюйте окремі напрямки.

---

## 🗺️ Загальна дорожня карта

```
Фаза 1 (місяці 1–3):  Фундамент
  → Мережі + ОС + Основи безпеки

Фаза 2 (місяці 4–8):  Технічне ядро
  → Безпека даних, програм, компонентів, з'єднань

Фаза 3 (місяці 9–14): Системний рівень
  → Безпека систем + практичні лаби

Фаза 4 (місяці 15–20): Організація та суспільство
  → Безпека людини, організаційна, суспільна

Фаза 5 (місяці 21+):  Сертифікація
  → CompTIA Security+ → CEH або CISSP
```

---

## 1. Безпека даних (Data Security)

*Основні теми: криптографія, цифрова криміналістика, цілісність та автентифікація, контроль доступу, захищені комунікації*

### 📚 Підручники та книги

| Назва | Автор | Рівень | Примітка |
|---|---|---|---|
| **Cryptography and Network Security: Principles and Practice** (8th ed.) | William Stallings | Середній | Класичний академічний підручник, охоплює симетричну/асиметричну криптографію, TLS, IPsec |
| **Serious Cryptography** | Jean-Philippe Aumasson | Середній–Просунутий | Практичний погляд на сучасну криптографію без зайвої математики |
| **The Code Book** | Simon Singh | Початковий | Захоплива історія криптографії від Цезаря до AES, чудово для мотивації |
| **Practical Forensic Imaging** | Bruce Nikkel | Середній | Цифрова криміналістика: збір доказів, образи дисків, ланцюжок зберігання |

### 🎓 Онлайн-курси

| Платформа | Курс | Вартість |
|---|---|---|
| **Coursera** | Cryptography I & II (Стенфорд, Dan Boneh) | Безкоштовно (аудит) |
| **edX / MIT OpenCourseWare** | Computer Systems Security (6.858) | Безкоштовно |
| **Cybrary** | Digital Forensics | Безкоштовно (базовий рівень) |

### 🛠️ Інструменти та лаби

- **TryHackMe** → Learning Path «Jr Penetration Tester» → секція Cryptography
- **CyberChef** (https://gchq.github.io/CyberChef/) — браузерний інструмент для криптографічних операцій, кодування, розбору форматів
- **Autopsy** — безкоштовна платформа цифрової криміналістики з відкритим кодом
- **Wireshark** — аналіз мережевих пакетів та захищених протоколів

---

## 2. Безпека програмного забезпечення (Software Security)

*Основні теми: принципи захищеного проектування, вимоги безпеки, реалізація, статичний/динамічний аналіз, розкриття вразливостей*

### 📚 Підручники та книги

| Назва | Автор | Рівень | Примітка |
|---|---|---|---|
| **The Web Application Hacker's Handbook** (2nd ed.) | Stuttard, Pinto | Середній | Охоплює OWASP Top 10, XSS, SQLi, CSRF — практично і вичерпно |
| **Writing Secure Code** (2nd ed.) | Howard, LeBlanc | Середній | Від Microsoft: принципи захищеного кодування для розробників |
| **Software Security: Building Security In** | Gary McGraw | Середній–Просунутий | Автор — член KAWG CSEC2017; Security в SDL |
| **The Art of Software Security Assessment** | Dowd, McDonald, Schuh | Просунутий | Глибокий аналіз коду та вразливостей |

### 🎓 Онлайн-курси

| Платформа | Курс | Вартість |
|---|---|---|
| **PortSwigger Web Security Academy** | Web Application Security (весь курс) | **Безкоштовно** |
| **Coursera** | Software Security (Університет Меріленду) | Безкоштовно (аудит) |
| **edX** | Secure Coding (NYU) | Безкоштовно (аудит) |
| **OWASP** | OWASP Testing Guide v4.2 (PDF) | **Безкоштовно** |

### 🛠️ Інструменти та лаби

- **PortSwigger Web Security Academy** (https://portswigger.net/web-security) — сотні безкоштовних лаб з реальними вразливостями
- **DVWA** (Damn Vulnerable Web Application) — навмисно вразливий застосунок для локального практикування
- **Burp Suite Community** — перехоплення та аналіз HTTP-трафіку
- **Semgrep** (безкоштовний) — статичний аналіз коду

---

## 3. Безпека компонентів (Component Security)

*Основні теми: вразливості компонентів, lifecycle, принципи захищеного проектування, ланцюг постачання, тестування, зворотна інженерія*

### 📚 Підручники та книги

| Назва | Автор | Рівень | Примітка |
|---|---|---|---|
| **The Hardware Hacker** | Andrew Huang («bunnie») | Середній | Апаратна безпека, виробництво, ланцюг постачання — від інсайдера |
| **Practical IoT Hacking** | Fotios Chantzis et al. | Середній | Безпека IoT-пристроїв та вбудованих систем |
| **Hacking: The Art of Exploitation** (2nd ed.) | Jon Erickson | Середній–Просунутий | Низькорівнева безпека: переповнення буферів, shellcode, експлойти |
| **Reversing: Secrets of Reverse Engineering** | Eldad Eilam | Просунутий | Зворотна інженерія бінарних файлів та ПЗ |

### 🎓 Онлайн-курси

| Платформа | Курс | Вартість |
|---|---|---|
| **Coursera** | Hardware Security (Університет Меріленду) | Безкоштовно (аудит) |
| **OpenSecurityTraining2** | Architecture 1001, Malware Analysis | **Безкоштовно** |
| **Ghidra Courses (NSA)** | Introduction to Ghidra | **Безкоштовно** |

### 🛠️ Інструменти та лаби

- **Ghidra** — безкоштовний інструмент зворотної інженерії від NSA
- **Radare2** — відкритий фреймворк для аналізу бінарних файлів
- **TryHackMe** → «Reverse Engineering» path
- **Hack The Box** → Reversing challenges

---

## 4. Безпека з'єднань (Connection Security)

*Основні теми: фізичні та програмні інтерфейси, мережева архітектура, атаки на з'єднання та передавання, захист мережі*

### 📚 Підручники та книги

| Назва | Автор | Рівень | Примітка |
|---|---|---|---|
| **Computer Networks** (6th ed.) | Andrew Tanenbaum | Початковий–Середній | Класика мережевих технологій, модель OSI, протоколи |
| **Network Security: Private Communication in a Public World** (2nd ed.) | Kaufman, Perlman, Speciner | Середній | TLS, IPsec, SSH, PKI — вичерпно |
| **Hacking: The Next Generation** | Dhanjani, Liu, Hardin | Середній | Реальні атаки на мережевий стек |
| **The Practice of Network Security Monitoring** | Richard Bejtlich | Середній | NSM, захоплення трафіку, аналіз інцидентів |

### 🎓 Онлайн-курси

| Платформа | Курс | Вартість |
|---|---|---|
| **Cisco Networking Academy** | CCNA (Introduction to Networks) | **Безкоштовно** |
| **Professor Messer** | CompTIA Network+ Course | **Безкоштовно** |
| **TryHackMe** | Pre-Security Path (Networking Fundamentals) | **Безкоштовно** |
| **Coursera** | The Bits and Bytes of Computer Networking (Google) | Безкоштовно (аудит) |

### 🛠️ Інструменти та лаби

- **Wireshark** — аналіз мережевих протоколів та пакетів
- **Nmap** — сканування мереж та виявлення сервісів
- **Metasploit Framework** — фреймворк для тестування на проникнення
- **GNS3 / Packet Tracer** — симулятори мережевого обладнання
- **TryHackMe** → «Network Fundamentals» + «Network Security» rooms

---

## 5. Безпека систем (System Security)

*Основні теми: цілісний підхід, політика безпеки, автентифікація, контроль доступу, моніторинг, відновлення, тестування*

### 📚 Підручники та книги

| Назва | Автор | Рівень | Примітка |
|---|---|---|---|
| **CompTIA Security+ Study Guide** (актуальне видання) | Mike Chapple, David Seidl | Початковий–Середній | Найкращий вступ до системної безпеки, відповідає доменам Security+ |
| **The Web Application Hacker's Handbook** | Stuttard, Pinto | Середній | Також охоплює системну безпеку вебзастосунків |
| **Linux Hardening in Hostile Networks** | Kyle Rankin | Середній | Практичне зміцнення Linux-систем |
| **Windows Security Internals** | James Forshaw | Просунутий | Внутрішня архітектура безпеки Windows |

### 🎓 Онлайн-курси

| Платформа | Курс | Вартість |
|---|---|---|
| **MIT OpenCourseWare** | Computer Systems Security (6.858) | **Безкоштовно** |
| **SANS** | SEC401: Security Essentials (платний, але матеріали публічні) | Платний |
| **Professor Messer** | CompTIA Security+ SY0-701 | **Безкоштовно** |
| **TryHackMe** | SOC Level 1 Path | Безкоштовно (частково) |

### 🛠️ Інструменти та лаби

- **TryHackMe** → «Jr SOC Analyst» path — SIEM, IDS, incident response
- **Splunk Free** — SIEM для аналізу журналів
- **Snort / Suricata** — системи виявлення вторгнень (IDS/IPS)
- **VirtualBox + Kali Linux** — безкоштовне середовище для локальних лабораторій
- **PicoCTF** (https://picoctf.org) — CTF-завдання від Carnegie Mellon для початківців

---

## 6. Безпека людини (Human Security)

*Основні теми: управління ідентичністю, соціальна інженерія, кібергігієна, конфіденційність персональних даних*

### 📚 Підручники та книги

| Назва | Автор | Рівень | Примітка |
|---|---|---|---|
| **The Art of Intrusion** | Kevin Mitnick | Початковий | Реальні кейси соціальної інженерії та фізичного проникнення |
| **Social Engineering: The Science of Human Hacking** (2nd ed.) | Christopher Hadnagy | Початковий–Середній | Систематичний підхід до соціальної інженерії та захисту від неї |
| **Data and Goliath** | Bruce Schneier | Початковий | Стеження, конфіденційність та захист персональних даних у цифрову епоху |
| **Spam Nation** | Brian Krebs | Початковий | Кіберзлочинність та її людський вимір |

### 🎓 Онлайн-курси

| Платформа | Курс | Вартість |
|---|---|---|
| **Coursera** | Usable Security (Університет Меріленду) | Безкоштовно (аудит) |
| **Cybrary** | Social Engineering | Безкоштовно |
| **SANS** | Security Awareness Training матеріали (публічні) | **Безкоштовно** |
| **iSC2** | Certified in Cybersecurity (CC) — безкоштовна сертифікація | **Безкоштовно** |

### 🛠️ Інструменти та лаби

- **SET (Social Engineering Toolkit)** у Kali Linux — фреймворк для навчальних симуляцій фішингу
- **Gophish** — безкоштовний фреймворк для симуляції фішингових кампаній
- **Have I Been Pwned** (https://haveibeenpwned.com) — перевірка витоків даних
- **Privacy Badger / uBlock Origin** — практичні інструменти захисту конфіденційності

---

## 7. Організаційна безпека (Organizational Security)

*Основні теми: управління ризиками, управління та політика, закони й етика, стратегія та планування*

### 📚 Підручники та книги

| Назва | Автор | Рівень | Примітка |
|---|---|---|---|
| **CISSP All-in-One Exam Guide** (актуальне видання) | Shon Harris, Fernando Maymí | Середній–Просунутий | Охоплює всі домени CISSP включно з управлінням ризиками |
| **How to Measure Anything in Cybersecurity Risk** | Hubbard, Seiersen | Середній | Кількісний підхід до вимірювання ризиків кібербезпеки |
| **The CISO Handbook** | Gentile, Bhatt, Bhatt | Середній | Практичний посібник для організаційних функцій безпеки |
| **Managing Cybersecurity Risk** | Jonathan Armstrong | Початковий–Середній | Корпоративне управління та регуляторний контекст |

### 🎓 Онлайн-курси

| Платформа | Курс | Вартість |
|---|---|---|
| **Coursera** | Cybersecurity and Its Ten Domains (Університет штату Джорджія) | Безкоштовно (аудит) |
| **NIST** | NIST Cybersecurity Framework 2.0 (офіційна документація) | **Безкоштовно** |
| **ISACA** | CISM Review Materials (частково публічні) | Частково безкоштовно |
| **edX** | Cybersecurity: Managing Risk in the Information Age (Гарвард) | Безкоштовно (аудит) |

### 🛠️ Стандарти та фреймворки (безкоштовні)

| Ресурс | URL | Що охоплює |
|---|---|---|
| **NIST CSF 2.0** | https://www.nist.gov/cyberframework | Управління ризиками, 6 функцій |
| **NIST SP 800-53** | https://csrc.nist.gov/publications | Каталог засобів контролю безпеки |
| **CIS Controls v8** | https://www.cisecurity.org/controls | 18 критичних засобів контролю |
| **MITRE ATT&CK** | https://attack.mitre.org | Тактики та техніки зловмисників |
| **ISO 27001 Overview** | https://www.iso.org/isoiec-27001-information-security.html | Система управління інформаційною безпекою |

---

## 8. Суспільна безпека (Societal Security)

*Основні теми: кіберзлочинність, кіберправо, кіберетика, кіберполітика, конфіденційність*

### 📚 Підручники та книги

| Назва | Автор | Рівень | Примітка |
|---|---|---|---|
| **Countdown to Zero Day** | Kim Zetter | Початковий | Stuxnet та кіберзброя — журналістська розслідувальна книга |
| **Sandworm** | Andy Greenberg | Початковий | Кібератаки на критичну інфраструктуру (Росія/Україна) — особливо актуально |
| **This Is How They Tell Me the World Ends** | Nicole Perlroth | Початковий | Ринок вразливостей нульового дня та кіберполітика |
| **Cybersecurity Law** (3rd ed.) | Jeff Kosseff | Середній | Автор — член KAWG CSEC2017; право у сфері кібербезпеки |
| **Future Crimes** | Marc Goodman | Початковий | Кіберзлочинність та її соціальний вплив |

### 🎓 Онлайн-курси

| Платформа | Курс | Вартість |
|---|---|---|
| **edX** | Cybersecurity: Managing Risk in the Information Age (Гарвард) | Безкоштовно (аудит) |
| **Coursera** | Cybersecurity Policy for Water and Electricity Infrastructures (Університет Дюка) | Безкоштовно (аудит) |
| **Future Learn** | Cyber Security: Safety at Home, Online, in Life (Newcastle) | Безкоштовно (аудит) |

### 🛠️ Ресурси та джерела

- **Krebs on Security** (https://krebsonsecurity.com) — авторитетний блог про кіберзлочинність
- **Recorded Future / CISA Alerts** (https://www.cisa.gov/news-events/cybersecurity-advisories) — поточні загрози
- **EFF (Electronic Frontier Foundation)** (https://www.eff.org) — конфіденційність та цифрові права
- **ENISA Threat Landscape** (https://www.enisa.europa.eu) — щорічний звіт про загрози в ЄС

---

## 🎓 Сертифікаційний шлях

Зіставлення сертифікацій із галузями знань CSEC2017:

| Рівень | Сертифікація | Покриття CSEC2017 | Вартість іспиту |
|---|---|---|---|
| **Базовий** | ISC2 CC (Certified in Cybersecurity) | Всі 8 KA (поверхово) | **Безкоштовно** |
| **Початковий** | CompTIA Security+ (SY0-701) | KA 1, 2, 4, 5, 7 | ~$392 |
| **Мережевий** | CompTIA Network+ | KA 4 (з'єднання) | ~$369 |
| **Аналітик** | CompTIA CySA+ | KA 5, 7 | ~$370 |
| **Етичний хакер** | CEH v13 | KA 1–5 | ~$950 |
| **Управлінський** | CISSP | KA 5–8 | ~$749 |
| **Тестування** | OSCP (Offensive Security) | KA 2–5 | ~$1499 |

**Рекомендований стартовий шлях для самостійного навчання:**
```
ISC2 CC (безкоштовно) → CompTIA Security+ → CySA+ або CEH
```

---

## 🖥️ Практичні платформи

| Платформа | URL | Кому підходить | Вартість |
|---|---|---|---|
| **TryHackMe** | https://tryhackme.com | Абсолютні початківці, структуровані шляхи | Безкоштовно / $14/міс |
| **Hack The Box** | https://hackthebox.com | Середній та просунутий рівень | Безкоштовно / $14/міс |
| **HTB Academy** | https://academy.hackthebox.com | Структуровані модулі за темами | Частково безкоштовно |
| **PortSwigger Web Security Academy** | https://portswigger.net/web-security | Безпека вебзастосунків | **Безкоштовно** |
| **PicoCTF** | https://picoctf.org | Початківці, CTF-завдання | **Безкоштовно** |
| **OverTheWire** | https://overthewire.org | Linux та основи безпеки | **Безкоштовно** |
| **Immersive Labs** | https://immersivelabs.com | Корпоративне середовище | Платний |

---

## 📰 Інформаційні ресурси для постійного моніторингу

| Ресурс | Тип | URL |
|---|---|---|
| **Krebs on Security** | Блог | https://krebsonsecurity.com |
| **Schneier on Security** | Блог | https://www.schneier.com |
| **The Hacker News** | Новини | https://thehackernews.com |
| **Dark Reading** | Новини | https://www.darkreading.com |
| **CISA Advisories** | Урядові сповіщення | https://www.cisa.gov/news-events/cybersecurity-advisories |
| **CVE Details** | База вразливостей | https://www.cvedetails.com |
| **MITRE ATT&CK** | Фреймворк загроз | https://attack.mitre.org |
| **SANS Internet Storm Center** | Щоденний моніторинг | https://isc.sans.edu |

---

## 📋 Рекомендовані безкоштовні матеріали для старту (Тиждень 1)

Якщо ви тільки починаєте і не знаєте, з чого почати — ось конкретний план на перший тиждень:

1. **Зареєструйтесь** на TryHackMe і пройдіть шлях «Pre-Security» (безкоштовно)
2. **Прочитайте** CSEC2017 Розділ 3 (концептуальна модель) — вже є у вашому перекладі
3. **Пройдіть** безкоштовний курс ISC2 CC на https://www.isc2.org/certifications/cc
4. **Перегляньте** відеокурс Professor Messer Security+ (YouTube, безкоштовно)
5. **Налаштуйте** VirtualBox + Kali Linux для локальних лабораторій

---

*Підбірка складена на основі CSEC2017 (Cybersecurity Curricula 2017, ACM/IEEE/AIS/IFIP). Останнє оновлення: 2025–2026.*
