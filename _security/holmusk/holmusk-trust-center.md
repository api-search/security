---
certifications:
- HITRUST CSF
- HIPAA / HITECH
description: ''
kind: trust-center
layout: security
name: Holmusk Trust Center
name_suffix: Trust Center
overview: Holmusk maintains a public trust center documenting HITRUST CSF and HIPAA / HITECH compliance.
provider_name: Holmusk
provider_slug: holmusk
slug: holmusk-trust-center
source_filename: holmusk-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nprobe: true\nurl: https://policy.holmusk.com/\ntitle: Holmusk HIPAA Compliance Policies\nsource: https://policy.holmusk.com/\nnote: >-\n  Holmusk does not run a conventional \"trust center\" (trust.holmusk.com does not resolve;\n  holmusk.com/trust, /security and /compliance all return 404). What it does publish — openly,\n  with no login — is its full HIPAA compliance policy set at policy.holmusk.com: ~176,000\n  characters covering policy management, risk management, roles, data management, system access,\n  incident response, breach notification, business continuity, configuration management and\n  vulnerability management, each section mapped to the HITRUST Common Security Framework control\n  and the HIPAA Security Rule citation it satisfies. That is a stronger public compliance artifact\n  than most trust pages, so it is recorded here.\ncertifications:\n- name: HITRUST CSF\n  status: claimed\n  evidence: >-\n    \"current production\
  \ systems on this platform are included in Holmusk's third-party audits and\n    HITRUST compliance\" — policy.holmusk.com §1.2 Compliance Inheritance. Every policy section\n    lists \"Applicable Standards from the HITRUST Common Security Framework\".\n- name: HIPAA / HITECH\n  status: claimed\n  evidence: >-\n    Policy set is structured as HIPAA Security Rule + HITECH Act control mappings\n    (e.g. 164.316(b)(1)(i), 13402(a)/(b)); Holmusk operates as a HIPAA business associate for\n    customer ePHI.\nnot_claimed:\n- name: SOC 2\n  note: >-\n    SOC 2 appears on policy.holmusk.com only as something Holmusk REVIEWS in its vendors\n    (\"annual assessment of SOC2 reports for all Holmusk infrastructure partners\"). Holmusk does\n    not claim a SOC 2 report of its own anywhere public, and it is not recorded as one here.\n- name: ISO 27001\n  note: Not mentioned on any public Holmusk surface probed on 2026-08-22.\naudit_reports:\n  public: false\n  detail: >-\n    \"Holmusk, at its sole\
  \ discretion, shares audit reports, including its HITRUST reports and\n    Corrective Action Plans (CAPs), with customers on a case by case basis. All audit reports are\n    shared under explicit NDA.\" — policy.holmusk.com §1.4\nhosting:\n  provider: Amazon Web Services\n  detail: Production infrastructure hosted on AWS; nginx web servers with Haskell, Java and NodeJS application servers (policy.holmusk.com §1.3).\nevidence:\n- source: https://policy.holmusk.com/\n  status: 200\n  keywords: [hipaa, hitrust, hitech, penetration testing, incident response, breach]\n- source: https://trust.holmusk.com/\n  status: DNS NXDOMAIN\n- source: https://www.holmusk.com/security\n  status: 404\n- source: https://www.holmusk.com/trust\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holmusk/refs/heads/main/security/holmusk-trust-center.yml
summary_line: HITRUST CSF, HIPAA / HITECH
tags:
- Company
- Healthcare
- Real-World Evidence
- Behavioral Health
- Mental Health
- Neuropsychiatry
- Clinical Data
- Data Analytics
- Life Sciences
- HIPAA
trust_url: https://policy.holmusk.com/
---
