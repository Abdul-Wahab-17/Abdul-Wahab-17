<div align="center">

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Abdul%20Wahab&fontSize=60&fontColor=ffffff&fontAlignY=38)

<a href="mailto:wahababdul7297@gmail.com">
  <img src="https://img.shields.io/badge/wahababdul7297%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
</a>
<a href="https://www.linkedin.com/in/abdul-wahab-mk/">
  <img src="https://img.shields.io/badge/abdul--wahab--mk-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
</a>

</div>

---

### About

Computer Science student at **SEECS, NUST** (graduating May 2027), building backend systems: APIs, data pipelines, and the infrastructure that serves ML models.

I've shipped backend services professionally, contributed tests to the SONiC network OS, and built ML systems end to end, from dataset construction to real-time inference. I care most about correctness, edge cases, and how systems behave under real-world load.

---

### Experience

**Software Engineer, Xandec** *(Jun 2026 – Sep 2026)*

- Built backend services and data processing pipelines for a client with NestJS, Next.js, PostgreSQL, Apache Kafka, Apache NiFi, and Redis.
- Documented REST APIs with Swagger/OpenAPI, containerized services with Docker, and set up GitLab CI/CD to automate testing and deployment.
- Benchmarked frontier LLMs, including Claude Opus 4.6 and GPT-5.5, on the Snorkel platform for quality, latency, and cost in enterprise AI workflows.

**Full Stack Developer, QWoods** *(Dec 2025 – Apr 2026)*

- Integrated WhatsApp messaging into the company's inventory management system to automate customer and operational communication.
- Built backend APIs and notification pipelines for inventory updates, order tracking, and stock alerts.

**Network Engineering Intern, ONT Lab, NUST** *(Jun 2025 – Sep 2025)*

- Wrote PTF-based automated tests for [SONiC](https://github.com/sonic-net) covering RX/TX counters, pause-frame handling, and control-plane packet behavior.
- Found an edge case where the `RX_DROP` counter increased on IEEE 802.3x (XON/XOFF) pause frames, and added a test to catch regressions.
- Test merged upstream: [sonic-net/sonic-mgmt#20543](https://github.com/sonic-net/sonic-mgmt/pull/20543)

---

### Projects

**[CardSense](https://github.com/Abdul-Wahab-17/CardSense)**: real-time card detection and Blackjack assistant

- Fine-tuned YOLOv8n on a 7,012-image custom and public dataset, reaching 87% mAP@0.5 at about 120 ms end-to-end latency.
- Distributed inference: a FastAPI backend queues camera frames on Redis Streams, and parallel YOLO workers consume them through a consumer group, scaling across machines and processes.
- Fuses hand and table camera feeds into one game state, smoothed with N-of-M frame consensus, and recommends legal moves from a rules engine with an optional LLM advisor.
- Streams live detections to a React dashboard over WebSockets; runs with Docker Compose and GitHub Actions CI.

`Python` `YOLOv8` `FastAPI` `Redis Streams` `WebSockets` `React` `Docker`

**[Factory Compliance System](https://github.com/Abdul-Wahab-17/FCS)**: AI safety monitoring for factory video

- Five-stage FastAPI pipeline: policy parsing, detection, severity classification, report generation, and escalation.
- Uses an LLM (via Groq) to turn a compliance policy PDF into structured rules, then cross-checks each rule against the PDF to catch hallucinations.
- YOLOv8 detects people, forklifts, and safety gear while CLIP infers scene context such as "hazardous zone"; findings are matched to the rules and graded LOW to CRITICAL.
- Pushes High and Critical violations to a React dashboard over WebSockets and stores every finding as an auditable report in SQLite. Tested with pytest and Dockerized.

`Python` `FastAPI` `YOLOv8` `CLIP` `OpenCV` `React` `SQLite` `Docker`

**[AgroYield](https://github.com/Abdul-Wahab-17/AgroYield)**: crop yield prediction

- Built a 3M+ record training set by joining USDA NASS yield, climate, and soil data at the county level.
- Trained and compared 10+ regression models, including Random Forest, XGBoost, LightGBM, and CatBoost, with leakage-safe preprocessing and temporal validation.
- Serves single-county and regional forecasts through a Flask API, with endpoints for model switching, metrics, and feature importance, behind a React dashboard.

`Python` `scikit-learn` `XGBoost` `LightGBM` `CatBoost` `Flask` `React`

**[TransitFlow](https://github.com/Abdul-Wahab-17/TransitFlow)**: transport management system

- Manages a transport service end to end: customers, drivers, vehicles, schedules, fees, and salaries.
- Role-based access with Spring Security for admins, drivers, customers, and a superadmin, each with their own dashboard.
- Layered controller → service → repository design on Spring Data JPA and MySQL, with Thymeleaf views for search, editing, activation toggles, and pending fee and salary reports.

`Java` `Spring Boot` `Spring Security` `Spring Data JPA` `Thymeleaf` `MySQL`

**[Memory-ECC](https://github.com/Abdul-Wahab-17/Memory-ECC)**: fault-tolerant memory for autonomous vehicles

- Simulates onboard vehicle memory protected by Hamming code (SEC-DED): corrects single-bit errors and detects double-bit errors.
- Runs periodic memory scrubbing to fix latent single-bit errors before they accumulate into uncorrectable ones.
- Includes fault injection, stress tests, and a GUI for watching errors get caught and corrected.

`Python` `Hamming code` `Fault injection`

---

### Technical Skills

**Languages:** Java · Python · C/C++ · JavaScript · Bash\
**Backend:** Spring Boot · NestJS · FastAPI · Express.js · Flask · Swagger/OpenAPI\
**Frontend:** React · Next.js · Tailwind CSS\
**Data & Messaging:** PostgreSQL · MySQL · MongoDB · Redis · Apache Kafka · Apache NiFi\
**Machine Learning:** PyTorch · TensorFlow · Keras · scikit-learn · Pandas · NumPy\
**DevOps:** Docker · GitLab CI/CD · Git · Linux\
**Networking:** SONiC · PTF · GNS3 · Packet capture analysis

---

### GitHub Stats

<div align="center">

  <img
    src="https://github-readme-stats.vercel.app/api?username=Abdul-Wahab-17&show_icons=true&theme=tokyonight&hide_border=true&count_private=true"
    height="180"
  />
  <img
    src="https://github-readme-stats.vercel.app/api/top-langs/?username=Abdul-Wahab-17&layout=compact&theme=tokyonight&hide_border=true"
    height="180"
  />

</div>

---

<div align="center">

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=100&section=footer)

</div>
