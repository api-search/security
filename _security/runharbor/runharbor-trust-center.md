---
certifications:
- 21 CFR Part 11
- HIPAA
- ICH E6 (GCP)
- ISPE GAMP 5
- ISO 13485
description: Harbor's security & compliance posture, captured from runharbor.com/security. As an eClinical platform handling ePHI and regulated clinical-trial data, Harbor operates as a HIPAA Business Associate (executes BAAs with clients) and designs the platform for 21 CFR Part 11 (unique user identification, immutable audit trails, electronic signatures). Validation is guided by ISPE GAMP 5 and ISO 13485, aligned to ICH E6 (GCP). No SOC 2, ISO 27001, or FedRAMP certification is claimed on the page. This is not a trust.<domain> subdomain trust center; it is the human-verified compliance posture from the /security page.
kind: trust-center
layout: security
name: Runharbor Trust Center
name_suffix: Trust Center
overview: Runharbor maintains a public trust center documenting 21 CFR Part 11, HIPAA, ICH E6 (GCP), ISPE GAMP 5, and ISO 13485 compliance.
provider_name: Runharbor
provider_slug: runharbor
slug: runharbor-trust-center
source_filename: runharbor-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: false\nsource: https://runharbor.com/security\nurl: https://runharbor.com/security\ndescription: >-\n  Harbor's security & compliance posture, captured from runharbor.com/security.\n  As an eClinical platform handling ePHI and regulated clinical-trial data,\n  Harbor operates as a HIPAA Business Associate (executes BAAs with clients) and\n  designs the platform for 21 CFR Part 11 (unique user identification, immutable\n  audit trails, electronic signatures). Validation is guided by ISPE GAMP 5 and\n  ISO 13485, aligned to ICH E6 (GCP). No SOC 2, ISO 27001, or FedRAMP\n  certification is claimed on the page. This is not a trust.<domain> subdomain\n  trust center; it is the human-verified compliance posture from the /security\n  page.\ncertifications:\n- {name: 21 CFR Part 11, scope: electronic records & signatures, note: unique user identification, immutable audit trails, e-signature workflows}\n- {name: HIPAA, role: Business\
  \ Associate, note: BAAs executed with clients; ePHI safeguards}\n- {name: ICH E6 (GCP), note: quality framework aligned with Good Clinical Practice}\n- {name: ISPE GAMP 5, note: risk-based computerized-system validation methodology}\n- {name: ISO 13485, note: medical-device quality-management alignment for validation}\nsecurity_controls:\n- Zero standing access; temporary access only via formal break-glass procedures\n- AES-256 encryption at rest; TLS 1.2+ in transit\n- Per-trial logically isolated dedicated databases\n- Hosted on Google Cloud Platform and AWS with private network architecture\ndocs:\n- https://runharbor.com/security\nevidence:\n- {source: https://runharbor.com/security, keywords: [21 cfr part 11, hipaa, ich e6, gamp 5, iso 13485, audit trail, encryption]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runharbor/refs/heads/main/security/runharbor-trust-center.yml
summary_line: 21 CFR Part 11, HIPAA, ICH E6 (GCP), ISPE GAMP 5, ISO 13485
tags:
- Company
- Clinical Trials
- Healthcare
- Contract Research Organization
- Electronic Data Capture
- Life Sciences
- Compliance
- Artificial Intelligence
- eClinical
trust_url: https://runharbor.com/security
---
