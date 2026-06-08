# B.Tech AIDS 2026 — Visual Curriculum Map

A semester-by-semester map of the AIDS 2026 scheme. **Each column is one semester.** Arrows show **prerequisite dependencies** (course at arrow tail is assumed knowledge for course at arrow head). Node colours encode **SIG alignment** (which Special Interest Group / specialization track a course feeds).

## How to read each node

Every node packs five facts:

```
CODE · Title
L-T-P-C | Category | Level
```

- **L-T-P-C** — Lecture-Tutorial-Practical-Credits
- **Category** — FC / HC / SC(PEC) / OE / ETC / MC / W (workshop) / AEC / Proj / Intern
- **Level** — A = awareness-floor course · Adv = has advanced ceiling · A+Adv = both · — = not graded on the dual-level scale (MC/AEC)

## SIG colour legend

| Colour | SIG / track |
|---|---|
| 🟦 Blue | Foundations & CSCore (common spine, placement-critical) |
| 🟪 Purple | AI/ML & Data Engineering SIG |
| 🟩 Teal | Agentic AI / Enterprise Applications SIG |
| 🟧 Amber | IoT · Blockchain · Process Automation SIG |
| 🟥 Pink | Cybersecurity Services SIG |
| ⬜ Grey | Humanities / Mandatory / Open (no SIG, no hard prereqs) |

---

## Curriculum dependency map

```mermaid
flowchart LR

  classDef found  fill:#E6F1FB,stroke:#185FA5,color:#042C53;
  classDef aiml   fill:#EEEDFE,stroke:#534AB7,color:#26215C;
  classDef agentic fill:#E1F5EE,stroke:#0F6E56,color:#04342C;
  classDef iot    fill:#FAEEDA,stroke:#854F0B,color:#412402;
  classDef cyber  fill:#FBEAF0,stroke:#993556,color:#4B1528;
  classDef gen    fill:#F1EFE8,stroke:#5F5E5A,color:#2C2C2A;

  subgraph S1["Semester 1"]
    direction TB
    S1_CALC["B24AS0103 · Multivariable Calculus & Linear Algebra<br/>3-0-0-3 | FC | A+Adv"]
    S1_C["B24CI0109 · Intro to C Programming<br/>1-1-0-2 | HC | A"]
    S1_CLAB["B24CI0110 · C Programming Lab<br/>0-0-1-1 | HC | A"]
    S1_PY["B25CS0101 · Python for Data Science<br/>2-0-0-2 | HC | A"]
    S1_PYLAB["B25CS0102 · Python for DS Lab<br/>0-0-1-1 | HC | A"]
    S1_EDL["B25EE0101 · Electronics & Digital Logic<br/>3-0-0-3 | HC | A+Adv"]
    S1_EXP["B24CSET01 · Engineering Exploration<br/>1-0-0-1 | HC | A"]
    S1_GEN1["FC/HSMC · Chem Tech · Civil Fund. · Finance & Mgmt<br/>FC | A"]
  end

  subgraph S2["Semester 2"]
    direction TB
    S2_PROB["B24AS0203 · Probability & Statistics<br/>3-0-0-3 | FC | A+Adv"]
    S2_ADVC["B25CI0201 · Advanced C with Generative AI<br/>1-1-1-3 | HC | A+Adv"]
    S2_BASD["B25CS0201 · Business Analysis & Software Design<br/>2-0-0-2 | HC | A"]
    S2_IOT["B24EN0101 · Internet of Things<br/>1-0-1-2 | HC | A+Adv"]
    S2_AIF["B25CSET01 · AI Foundations for Engineers<br/>1-0-0-1 | ETC | A"]
    S2_INE["B24ME0102 · Innovation & Entrepreneurship<br/>1-0-1-2 | FC | A"]
    S2_PHY["B24AS0106 · Physics for CS (+Lab)<br/>FC | A"]
    S2_GEN2["FC/HSMC · Mech Eng · Communicative English<br/>FC | A"]
  end

  subgraph S3["Semester 3"]
    direction TB
    S3_DM["B25AS0301 · Discrete Maths & Graph Theory<br/>3-0-0-3 | FC | A+Adv"]
    S3_DSA["B25CS0301 · Data Structures & Algorithms<br/>1-1-1-3 | HC | A+Adv"]
    S3_DBMS["B25CS0302 · Database Management Systems<br/>1-1-1-3 | HC | A+Adv"]
    S3_OOP["B25EA0301 · OOP with Python<br/>2-1-1-4 | HC | A+Adv"]
    S3_AI["B25EA0302 · Principles of AI<br/>3-0-0-3 | HC | A+Adv"]
    S3_PORT["B25EA0303 · Portfolio Development (W1)<br/>0-0-2-2 | W | A"]
    S3_WEB["B25EA0304 · App Dev-1: Web Design (W2)<br/>0-0-2-2 | W | A+Adv"]
    S3_AEC1["B25CS0305 · Placement Training (AEC-1)<br/>0-0-1-1 | AEC | —"]
    S3_DT["B25CS0304 · Design Thinking<br/>0-0-1-1 | HC | A"]
  end

  subgraph S4["Semester 4"]
    direction TB
    S4_OPT["Optimization Techniques<br/>3-0-0-3 | HC | A+Adv"]
    S4_DAA["Design & Analysis of Algorithms<br/>1-1-1-3 | HC | A+Adv"]
    S4_SML["Statistical Machine Learning<br/>1-1-1-3 | HC | A+Adv"]
    S4_JAVA["Java<br/>1-1-1-3 | HC | A+Adv"]
    S4_ADBMS["App Dev-2: Advanced DBMS (W3)<br/>0-0-2-2 | W | A+Adv"]
    S4_DE["Data Engineering (W4)<br/>0-0-2-2 | W | A+Adv"]
    S4_COA["MOOC/NPTEL: Computer Organization<br/>0-0-2-2 | HC | A"]
    S4_AEC2["Placement Training (AEC-2)<br/>0-0-1-1 | AEC | —"]
  end

  subgraph S5["Semester 5"]
    direction TB
    S5_NLP["Natural Language Processing<br/>2-0-1-3 | HC | A+Adv"]
    S5_OS["Operating Systems<br/>2-0-1-3 | HC | A+Adv"]
    S5_DL["Deep Learning<br/>1-1-1-3 | HC | A+Adv"]
    S5_MP1["Mini Project-1<br/>0-0-2-2 | Proj | A+Adv"]
    S5_PE1["PE-1 · DS for X (BFSI/Energy/Aero) / LLM Engineering<br/>3-0-0-3 | SC | Adv"]
    S5_OE1["Open Elective-1<br/>3-0-0-3 | OE | A"]
    S5_DV["Data Visualization (W5)<br/>0-0-2-2 | W | A+Adv"]
    S5_MLOPS["MLOps (W6)<br/>0-0-2-2 | W | A+Adv"]
    S5_AEC3["Placement Training (AEC-3)<br/>0-0-1-1 | AEC | —"]
  end

  subgraph S6["Semester 6"]
    direction TB
    S6_CLOUD["Principles of Cloud Computing<br/>2-1-0-3 | HC | A+Adv"]
    S6_GENAI["Generative AI<br/>1-1-1-3 | HC | A+Adv"]
    S6_CN["Computer Networks<br/>1-1-1-3 | HC | A+Adv"]
    S6_PE2["PE-2 · DS for X (Functional) / LLMOps<br/>3-0-0-3 | SC | Adv"]
    S6_OE2["Open Elective-2<br/>3-0-0-3 | OE | A"]
    S6_BDA["Big Data Analytics (W7)<br/>0-0-2-2 | W | A+Adv"]
    S6_AIAPP["AI App Dev (W8)<br/>0-0-2-2 | W | A+Adv"]
    S6_MP2["Mini Project-2<br/>0-0-3-3 | Proj | A+Adv"]
    S6_AEC4["Placement Training (AEC-4)<br/>0-0-1-1 | AEC | —"]
  end

  subgraph S7["Semester 7"]
    direction TB
    S7_PE3["PE-3 · Edge AI & Federated Learning / Agentic AI<br/>3-0-0-3 | SC | Adv"]
    S7_PE4["PE-4 · HPC in DS / Multimodal LLM<br/>3-0-0-3 | SC | Adv"]
    S7_CAP1["Capstone Project Phase-I<br/>0-0-8-8 | Proj | A+Adv"]
    S7_INT1["Internship<br/>0-0-4-4 | Intern | A+Adv"]
    S7_CERT["Global Certification<br/>0-0-1-2 | Proj | Adv"]
  end

  subgraph S8["Semester 8"]
    direction TB
    S8_PE5["PE-5 · Large Action Models / Frontiers of AI / Ethical AI<br/>3-0-0-3 | SC | Adv"]
    S8_PE6["PE-6 · DS for Cybersecurity / DS for IoT / Adversarial AI<br/>3-0-0-3 | SC | Adv"]
    S8_CAP2["Capstone Project Phase-II<br/>0-0-3-3 | Proj | A+Adv"]
    S8_INT2["Internship<br/>0-0-4-4 | Intern | A+Adv"]
  end

  %% ---- Prerequisite dependency arrows ----

  %% Programming spine
  S1_C --> S1_CLAB
  S1_PY --> S1_PYLAB
  S1_C --> S2_ADVC
  S1_PY --> S2_ADVC
  S1_PY --> S3_OOP
  S2_ADVC --> S3_OOP
  S3_OOP --> S4_JAVA

  %% Data structures / algorithms chain
  S1_C --> S3_DSA
  S1_CLAB --> S3_DSA
  S3_DSA --> S3_DBMS
  S3_DSA --> S4_DAA
  S3_DM --> S4_DAA
  S3_DM --> S3_DSA
  S4_OPT --> S4_DAA

  %% Database / data engineering chain
  S3_DBMS --> S4_ADBMS
  S4_ADBMS --> S4_DE
  S4_DE --> S6_BDA
  S2_BASD --> S3_DBMS

  %% AI / ML / DL chain
  S1_CALC --> S2_PROB
  S2_PROB --> S4_SML
  S3_AI --> S4_SML
  S2_AIF --> S3_AI
  S4_SML --> S5_DL
  S4_OPT --> S5_DL
  S5_DL --> S5_NLP
  S5_DL --> S6_GENAI
  S5_NLP --> S6_GENAI

  %% MLOps / data viz / app dev
  S4_DE --> S5_MLOPS
  S5_DL --> S5_MLOPS
  S2_PROB --> S5_DV
  S3_WEB --> S6_AIAPP
  S6_GENAI --> S6_AIAPP

  %% Systems chain
  S4_COA --> S5_OS
  S5_OS --> S6_CN
  S5_OS --> S6_CLOUD
  S6_CN --> S6_CLOUD

  %% IoT chain
  S1_EDL --> S2_IOT

  %% Projects / capstone / internship progression
  S5_DL --> S5_MP1
  S5_MP1 --> S6_MP2
  S6_MP2 --> S7_CAP1
  S7_CAP1 --> S8_CAP2
  S7_INT1 --> S8_INT2
  S6_AIAPP --> S7_CAP1

  %% Professional elective progression (SIG tracks)
  S5_PE1 --> S6_PE2
  S6_PE2 --> S7_PE3
  S7_PE3 --> S7_PE4
  S7_PE4 --> S8_PE5
  S8_PE5 --> S8_PE6
  S5_DL --> S5_PE1
  S6_GENAI --> S7_PE3

  %% ---- SIG colour assignments ----

  class S1_CALC,S1_C,S1_CLAB,S1_PY,S1_PYLAB,S1_EDL,S1_EXP,S2_PROB,S2_ADVC,S2_BASD,S2_AIF,S3_DM,S3_DSA,S3_DBMS,S3_OOP,S3_DT,S3_AEC1,S4_OPT,S4_DAA,S4_JAVA,S4_COA,S4_AEC2,S5_OS,S5_AEC3,S6_CN,S6_AEC4,S3_PORT found
  class S3_AI,S4_SML,S5_NLP,S5_DL,S5_DV,S5_MLOPS,S6_GENAI,S5_PE1,S6_PE2,S7_PE4,S8_PE5,S5_MP1 aiml
  class S3_WEB,S4_ADBMS,S4_DE,S6_BDA,S6_AIAPP,S6_CLOUD,S7_PE3,S6_MP2,S7_CAP1,S8_CAP2,S7_INT1,S8_INT2,S7_CERT agentic
  class S1_EDL,S2_IOT iot
  class S8_PE6 cyber
  class S1_GEN1,S2_INE,S2_PHY,S2_GEN2,S5_OE1,S6_OE2 gen
```

---

## Notes on the map

**Dependencies shown are academic prerequisites**, not administrative sequencing. An arrow means the source course supplies knowledge the target course assumes. Soft or motivational links (e.g. Design Thinking → projects) are omitted to keep the prerequisite signal clean.

**Three backbone chains** are visible if you trace the arrows:

- *Programming → OOP → Java* (the language/software spine, blue → feeding AI/ML).
- *Calculus → Probability → Statistical ML → Deep Learning → NLP / Generative AI* (the AI/ML spine, purple).
- *DBMS → Advanced DBMS → Data Engineering → Big Data / AI App Dev → Capstone* (the data/enterprise spine, teal).

**SIG colour reflects where a course leads**, not only what it teaches. Foundation and CSCore courses are blue because they are the common placement-critical spine every SIG depends on; the professional electives fan out into their SIG colours from Semester 5 onward, which is exactly where students choose tracks (informed by performance feedback, per the strategy).

**Professional electives (PE-1…PE-6)** each list their T1/T2 choices in the node. The colour assigned is the *dominant* SIG, but several electives are genuinely cross-SIG — e.g. PE-6 (DS for Cybersecurity / DS for IoT / Adversarial AI) spans the Cybersecurity and IoT SIGs; it is coloured by its cyber option here.

**Greyed/condensed nodes** (humanities, mandatory courses, physics, open electives) carry no hard prerequisites and no SIG alignment, so they are shown condensed rather than as separate dependency nodes — including Indian Constitution & Cyber Law, Environmental Science, Universal Human Values, Professional Ethics, IKS, and the AEC placement-training thread (which runs every semester 3–6 as the CSCore spine).

**Workshops (W1–W8)** appear as graded nodes because in this scheme they carry credits and have real prerequisites — but recall their titles are *indicative*: the SIG teams design the actual content just-in-time, so the arrows show the skill dependency, not a frozen syllabus.
