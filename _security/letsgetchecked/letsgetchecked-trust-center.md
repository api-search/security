---
certifications:
- GDPR
- HITRUST
- NIST
- ISO 13485
description: ''
kind: trust-center
layout: security
name: Letsgetchecked Trust Center
name_suffix: Trust Center
overview: LetsGetChecked maintains a public trust center documenting GDPR, HITRUST, NIST, and ISO 13485 compliance.
provider_name: LetsGetChecked
provider_slug: letsgetchecked
slug: letsgetchecked-trust-center
source_filename: letsgetchecked-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nsource: https://trust.letsgetchecked.com/\nurl: https://trust.letsgetchecked.com/\nplatform: Conveyor\npublished: true\nclaimed_by_vendor: true\n\n# CORRECTION NOTE (2026-08-04): the mechanical keyword probe first recorded\n# SOC 2 / ISO 27001 / ISO 27017 / ISO 27018 / FedRAMP for LetsGetChecked. Those are\n# WRONG. The Conveyor trust-center page embeds a \"trusted by / vendors\" data blob\n# carrying OTHER companies' certification lists (Salesforce, Twilio, AWS, Mailgun,\n# Lob, PFL, Momentive), and the keyword scan picked those up. The list below is taken\n# from LetsGetChecked's OWN record in the page's window.CANONICAL_ASSET object\n# (id 0d8b479f-ac02-4970-80ea-91d7dd5935d4, slug \"letsgetchecked\",\n# website http://www.letsgetchecked.com), which is the authoritative vendor entry.\n# Do not re-run the keyword probe over this file without re-applying this correction.\n\ncertifications:\n- GDPR\n- HITRUST\n- NIST\n\
  - ISO 13485\n\ncertifications_raw:\n- gdpr\n- hitrust\n- nist\n- iso-13485\n\nnot_claimed:\n  note: 'Absent from the vendor''s own certification list on its trust centre. Recorded\n    because a healthcare data processor is commonly assumed to hold these.'\n  frameworks:\n  - SOC 2 Type II\n  - ISO 27001\n  - HIPAA\n  hipaa_note: 'HIPAA is not listed as a certification on the trust centre, though the\n    API documentation discusses PHI handling and the developer glossary defines PHI\n    under HIPAA.'\n  soc2_indicator: 'Conveyor''s own trust indicator \"Do they have a current SOC 2 Type\n    II Report to share (or proof that they support a comparable framework)?\" scores\n    \"unknown\" on this profile — no data collected.'\n\nreport_vulnerability_url: https://www.letsgetchecked.com/security.txt\nhas_published_report: false\npublic_profile_published: true\nsubprocessors_published: true\nsubprocessors_updated_at: '2025-11-14T17:00:19.811Z'\nsubprocessor_count: 14\nsubprocessor_categories:\n\
  - Telephony management\n- Cloud service provider\n- Customer communications\n- Lab Information System\n- Prescription System\n- Email & document storage\n- Mail Provider\n- Transactional Email provider\n- eFax provider\n- CRM\n- Supporting Onsite Health Screening\n- Email encryption\nsubprocessor_data_locations:\n- United States\nsections:\n- Featured Documents\n- What we offer\n- Subprocessors\n- Video Resources\nlast_updated: '2025-12-15T20:27:33.184Z'\n\nevidence:\n- source: https://trust.letsgetchecked.com/\n  http_status: 200\n  fetched: '2026-08-04'\n  extracted_from: window.CANONICAL_ASSET (the vendor's own record on the Conveyor page)\n  fields:\n  - certifications\n  - report_vulnerability_url\n  - subprocessors\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/letsgetchecked/refs/heads/main/security/letsgetchecked-trust-center.yml
summary_line: GDPR, HITRUST, NIST, ISO 13485
tags:
- Company
- Health
- Healthcare
- Diagnostics
- Laboratory
- Telehealth
- Medical Testing
- Pharmacy
- Order
- Results
- Webhook
- HL7
- LOINC
trust_url: https://trust.letsgetchecked.com/
---
