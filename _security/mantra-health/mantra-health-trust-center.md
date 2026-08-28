---
certifications:
- HIPAA
- SOC 2
- SOC 1
- TX-RAMP
description: ''
kind: trust-center
layout: security
name: Mantra Health Trust Center
name_suffix: Trust Center
overview: Mantra Health maintains a public trust center documenting HIPAA, SOC 2, SOC 1, and TX-RAMP compliance.
provider_name: Mantra Health
provider_slug: mantra-health
slug: mantra-health-trust-center
source_filename: mantra-health-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://mantrahealth.com/security-and-privacy/\nname: Mantra Health security and compliance\nnote: >-\n  Mantra Health does not run a trust center in the modern sense — there is no trust.mantrahealth.com,\n  no Vanta/Drata/SafeBase portal, and no document request flow. What it publishes is a single\n  marketing-site page, \"Security and Privacy at Mantra Health\", naming three compliance frameworks in\n  prose. That page is the whole of the public posture, and it is recorded here verbatim. The\n  automated probe (probe-security-programs.py) missed it because the page sits at\n  /security-and-privacy/ rather than any of the conventional /trust, /security, /compliance paths;\n  /security does 302 to it, which is how it was found.\ntrust_center:\n  present: partial\n  url: https://mantrahealth.com/security-and-privacy/\n  http_status: 200\n  type: marketing-page\n  portal: false\n  document_request_flow: false\n  document_request_note:\
  \ >-\n    No mechanism to request a SOC report, questionnaire response or subprocessor list. The page's only\n    call to action is the generic \"Get in Touch\" sales form at https://mantrahealth.com/get-in-touch/.\n  subprocessors_published: false\n  pen_test_published: false\n  uptime_sla_published: false\ncertifications:\n- name: HIPAA\n  status: self-attested\n  evidence_quote: >-\n    \"We adhere to the national standard for handling Protected Health Information (PHI) related to\n    student health records, medical research collaborations, and other university-related healthcare\n    data.\"\n  certificate_published: false\n  date: null\n- name: SOC 2\n  status: claimed-audited\n  evidence_quote: >-\n    \"Mantra has undergone a rigorous external audit, in which our security, availability, processing\n    integrity, confidentiality, and privacy controls have been assessed and approved.\"\n  certificate_published: false\n  auditor: null\n  report_type: null\n  report_type_note: The\
  \ page does not state whether the report is Type I or Type II, nor its period.\n  date: null\n- name: SOC 1\n  status: claimed-audited\n  evidence_quote: '\"SOC-I & SOC-II\" (page heading)'\n  certificate_published: false\n  date: null\n- name: TX-RAMP\n  status: claimed-aligned\n  evidence_quote: >-\n    \"We're proactively committed to aligning with state-specific security requirements, including the\n    TX RMP security framework which is mandated for higher education institutions and state agencies\n    in Texas.\"\n  certificate_published: false\n  note: >-\n    Stated as alignment/commitment, not as a granted certification at a level. No TX-RAMP\n    certification number or status is published.\n  date: null\nnot_claimed:\n- name: ISO 27001\n  note: Not mentioned anywhere on the page or site.\n- name: HITRUST CSF\n  note: >-\n    Not mentioned. Notable only because HITRUST is the common companion certification for a HIPAA\n    covered entity or business associate at this size; its\
  \ absence is recorded, not judged.\n- name: FERPA\n  note: >-\n    Not mentioned, despite student education records being squarely in scope for a vendor to colleges\n    and universities.\n- name: FedRAMP\n  note: Not mentioned.\n- name: PCI DSS\n  note: Not mentioned; no evidence Mantra handles cardholder data (it bills institutions, not students).\nobserved_technical_posture:\n  note: >-\n    Independently probed, and corroborating the compliance claims: api.mantrahealth.com returns HSTS\n    (max-age 31536000, includeSubDomains), a restrictive Content-Security-Policy, X-Frame-Options\n    DENY, X-Content-Type-Options nosniff, X-XSS-Protection, X-Download-Options and\n    Surrogate-Control no-store. The registrable domain publishes SPF and a DMARC policy of p=reject.\n    DNSSEC is not enabled and no CAA record is published. See\n    security/mantra-health-domain-security.yml.\n  cross_ref: security/mantra-health-domain-security.yml\nevidence:\n- url: https://mantrahealth.com/security-and-privacy/\n\
  \  status: 200\n- url: https://mantrahealth.com/security\n  status: 200\n  note: 302 to /security-and-privacy/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mantra-health/refs/heads/main/security/mantra-health-trust-center.yml
summary_line: HIPAA, SOC 2, SOC 1, TX-RAMP
tags:
- Company
- Health Care
- Mental Health
- Telehealth
- Higher Education
- Digital Health
- Patient Engagement
- HIPAA
- GraphQL
trust_url: ''
---
