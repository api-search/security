---
certifications:
- PCI DSS Level 1
- ISO/IEC 27001
- ISO 22301
description: ''
kind: trust-center
layout: security
name: Trainline Trust Center
name_suffix: Trust Center
overview: Trainline maintains a public trust center documenting PCI DSS Level 1, ISO/IEC 27001, and ISO 22301 compliance.
provider_name: Trainline
provider_slug: trainline
slug: trainline-trust-center
source_filename: trainline-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nprobe: true\nurl: https://www.thetrainline.com/terms/security\ntitle: Trainline Security Overview\nnote: >-\n  Trainline runs no vendor trust portal (no trust.thetrainline.com, no Vanta/Drata/SafeBase\n  page, no security.thetrainline.com). Its published trust surface is a single consumer-facing\n  \"Trainline Security Overview\" page under the terms tree. It is unusually substantive for that\n  format — it names certifications with certificate numbers, an uptime commitment, the hosting\n  provider and data residency, and a vulnerability reporting address — so it is captured here as\n  the trust-centre equivalent. There is no partner/API-specific trust pack published, and no\n  downloadable evidence (no SOC 2 report, no ISO certificate PDF, no CAIQ/SIG, no subprocessor list).\ncertifications:\n  - name: PCI DSS Level 1\n    scope: both as a merchant and as a service provider\n    quote: \"Trainline are PCI Level 1 compliant both as\
  \ a merchant and as a service provider\"\n    certificate_number: null\n  - name: ISO/IEC 27001\n    scope: Information Security Management Systems\n    certificate_number: IS 775108\n  - name: ISO 22301\n    scope: Business Continuity Management Systems\n    certificate_number: BCMS 763415\nregulatory:\n  - name: UK GDPR / EU GDPR\n    posture: >-\n      \"We're strong advocates of the GDPR and believe that the transparency it delivers around\n      the management and use of personal data is great for our customers, partners and our staff.\"\n    privacy_policy: https://www.thetrainline.com/terms/privacy\n    data_subject_contact: DPO@thetrainline.com\n  - name: Modern Slavery Act (UK)\n    posture: statement published in the site footer\nnot_published:\n  - SOC 2 Type I / Type II\n  - ISO 27017 / ISO 27018\n  - Cyber Essentials / Cyber Essentials Plus\n  - HIPAA\n  - FedRAMP\n  - CSA STAR / CAIQ\n  - subprocessor list\n  - downloadable audit evidence or NDA-gated evidence portal\ninfrastructure:\n\
  \  hosting: Amazon Web Services (AWS)\n  data_residency: European Economic Area (EEA)\n  quote: >-\n    \"We protect our systems and your data within industry-leading, accredited data centres,\n    operated by Amazon Web Services (AWS), which are located in the European Economic Area (EEA).\"\n  resilience: >-\n    \"Our systems are mirrored across multiple sites (AWS availability zones), each of which have\n    backup power supplies and networks.\"\navailability_commitment:\n  uptime_target: 99.9%\n  quote: >-\n    \"We provide a commitment to our customers that our services will achieve at least 99.9%\n    operational uptime.\"\n  scope: consumer services as described on the security overview page; no API-specific SLA is published\n  contractual: false\ncontrols:\n  governance: dedicated Information Security team\n  personnel: BPSS security screening for all staff, contractors and temporary workers\n  training: regular security and privacy training for all staff; annual secure code training\
  \ for engineers\n  supply_chain: Supplier Security team; compliance screening and contractual security/data-privacy obligations\n  operational: Advanced Web Application Firewall, DDoS protection, bot management, anti-virus/anti-malware, IDS/IPS, 24/7 SOC\n  secure_sdlc: BSIMM-based software security programme; static and dynamic code analysis\nevidence:\n  - source: https://www.thetrainline.com/terms/security\n    status: 200\n    keywords: [pci level 1, iso 27001, iso 22301, gdpr, information security, penetration testing, soc]\n  - source: https://trust.thetrainline.com\n    status: 000\n    note: does not resolve\n  - source: https://www.trainlinegroup.com/security\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trainline/refs/heads/main/security/trainline-trust-center.yml
summary_line: PCI DSS Level 1, ISO/IEC 27001, ISO 22301
tags:
- Travel
- Rail
- United Kingdom
- Europe
- Booking
- Ticketing
- Distribution
- OTA
- Corporate Travel
trust_url: https://www.thetrainline.com/terms/security
---
