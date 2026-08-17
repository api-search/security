---
api_specs:
- filename: health-gorilla-binary-api-openapi.yml
  format: yaml
  label: Health Gorilla Binary API
  slug: health-gorilla-binary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-binary-api-openapi.yml
- filename: health-gorilla-capabilitystatement-api-openapi.yml
  format: yaml
  label: Health Gorilla CapabilityStatement API
  slug: health-gorilla-capabilitystatement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-capabilitystatement-api-openapi.yml
- filename: health-gorilla-coverage-api-openapi.yml
  format: yaml
  label: Health Gorilla Coverage API
  slug: health-gorilla-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-coverage-api-openapi.yml
- filename: health-gorilla-diagnosticreport-api-openapi.yml
  format: yaml
  label: Health Gorilla DiagnosticReport API
  slug: health-gorilla-diagnosticreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-diagnosticreport-api-openapi.yml
- filename: health-gorilla-documentreference-api-openapi.yml
  format: yaml
  label: Health Gorilla DocumentReference API
  slug: health-gorilla-documentreference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-documentreference-api-openapi.yml
- filename: health-gorilla-observation-api-openapi.yml
  format: yaml
  label: Health Gorilla Observation API
  slug: health-gorilla-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-observation-api-openapi.yml
- filename: health-gorilla-patient-api-openapi.yml
  format: yaml
  label: Health Gorilla Patient API
  slug: health-gorilla-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-patient-api-openapi.yml
- filename: health-gorilla-practitioner-api-openapi.yml
  format: yaml
  label: Health Gorilla Practitioner API
  slug: health-gorilla-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-practitioner-api-openapi.yml
- filename: health-gorilla-requestgroup-api-openapi.yml
  format: yaml
  label: Health Gorilla RequestGroup API
  slug: health-gorilla-requestgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-requestgroup-api-openapi.yml
- filename: health-gorilla-servicerequest-api-openapi.yml
  format: yaml
  label: Health Gorilla ServiceRequest API
  slug: health-gorilla-servicerequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-servicerequest-api-openapi.yml
certifications:
- HITRUST r2
- SOC 2 Type 2
- HIPAA
description: Health Gorilla publishes a Health Data Security page naming its certifications, its identity-assurance standard and its encryption posture. There is no dedicated trust portal (trust.healthgorilla.com does not resolve) and no self-serve document request; the security posture is stated on a marketing page rather than in a Vanta/Drata-style trust center. The certifications named are specific, dated by accompanying company blog announcements, and consistent with the company's TEFCA QHIN designation.
kind: trust-center
layout: security
name: Health Gorilla Trust Center
name_suffix: Trust Center
overview: Health Gorilla maintains a public trust center documenting HITRUST r2, SOC 2 Type 2, and HIPAA compliance.
provider_name: Health Gorilla
provider_slug: health-gorilla
slug: health-gorilla-trust-center
source_filename: health-gorilla-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://www.healthgorilla.com/home/company/health-data-security\ndescription: >-\n  Health Gorilla publishes a Health Data Security page naming its certifications,\n  its identity-assurance standard and its encryption posture. There is no\n  dedicated trust portal (trust.healthgorilla.com does not resolve) and no\n  self-serve document request; the security posture is stated on a marketing page\n  rather than in a Vanta/Drata-style trust center. The certifications named are\n  specific, dated by accompanying company blog announcements, and consistent with\n  the company's TEFCA QHIN designation.\nurl: https://www.healthgorilla.com/home/company/health-data-security\nportal_type: security page (no dedicated trust portal)\ncertifications:\n- name: HITRUST r2\n  full_name: HITRUST Risk-based, 2-year Certification\n  status: certified\n  evidence: >-\n    \"We're HITRUST R2 certified, which means that we successfully\
  \ manage\n    cybersecurity risks by exceeding industry-defined information security\n    requirements.\"\n  announcement: https://www.healthgorilla.com/blog/strengthening-our-security-canopy-health-gorilla-earns-hitrust-r2-recertification\n- name: SOC 2 Type 2\n  status: certified\n  trust_service_criteria: [security, availability, processing integrity, confidentiality, privacy]\n  evidence: >-\n    \"SOC 2 Type 2 is a stamp of approval on our controls relevant to data\n    security, availability, processing, integrity, confidentiality, and privacy.\"\n  announcement: https://www.healthgorilla.com/blog/health-gorilla-is-now-soc-2-type-2-certified\n- name: HIPAA\n  status: compliance program\n  evidence: >-\n    \"Complying with applicable health data laws, including HIPAA, is ingrained in\n    our culture, processes, and staff training.\"\nframeworks:\n- name: NIST SP 800-63A IAL2\n  description: >-\n    Identity verified to Identity Assurance Level 2 as specified in NIST Special\n  \
  \  Publication 800-63A, described as one of the highest forms of personal\n    verification.\n- name: TEFCA\n  description: >-\n    Designated Qualified Health Information Network operating under the Trusted\n    Exchange Framework and Common Agreement and its Recognized Coordinating Entity.\n- name: CalHHS Data Exchange Framework\n  description: Designated Qualified Health Information Organization in California.\ncontrols_published:\n- {control: Encryption in transit and at rest, description: 'Medical records are encrypted in transit and at rest.'}\n- {control: Credential handling, description: 'Passwords are not stored on a web server and are end-to-end encrypted.'}\n- {control: Backup, description: 'Retrieved patient health information is backed up on the secure cloud platform.'}\n- {control: TLS floor, description: 'All API access requires TLS 1.2 or higher; plain HTTP is rejected.', source: 'https://developer.healthgorilla.com/reference/fhir-versions'}\nnot_found:\n  trust_portal:\
  \ https://trust.healthgorilla.com\n  trust_portal_result: DNS does not resolve (curl exit 6)\n  document_request_flow: none published\n  subprocessor_list: none found\n  pentest_report: none published\n  iso_27001: not claimed\n  fedramp: not claimed\n  soft_404_warning: >-\n    www.healthgorilla.com is a Webflow catch-all that answers HTTP 200 with the\n    same 70,722-byte site shell for every unknown path — /security, /compliance,\n    /trust-center and /legal/privacy-policy all returned that shell and are NOT\n    real pages. Only the /home/* paths listed in the sitemap are genuine.\nrelated:\n- conformance/health-gorilla-conformance.yml\n- security/health-gorilla-vulnerability-disclosure.yml\n- security/health-gorilla-domain-security.yml\nevidence:\n- {source: 'https://www.healthgorilla.com/home/company/health-data-security', http_status: 200, keywords: [HITRUST R2, SOC 2 Type 2, HIPAA, NIST 800-63A, IAL2, end-to-end encryption]}\n- {source: 'https://www.healthgorilla.com/sitemap.xml',\
  \ http_status: 200, note: 'used to distinguish real pages from the Webflow soft-404 shell'}\nx-evidence:\n- {url: 'https://www.healthgorilla.com/home/company/health-data-security', http_status: 200, fetched: '2026-08-14'}\n- {url: 'https://www.healthgorilla.com/trust-center', http_status: 200, fetched: '2026-08-14', note: 'soft-404 shell — rejected'}\n- {url: 'https://trust.healthgorilla.com', http_status: 0, fetched: '2026-08-14', note: 'DNS does not resolve'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/security/health-gorilla-trust-center.yml
summary_line: HITRUST r2, SOC 2 Type 2, HIPAA
tags:
- Health
- Interoperability
- FHIR
- Clinical Data
- Lab Ordering
- TEFCA
- QHIN
- Health Information Exchange
- Lab Results
- Clinical Documents
- SMART on FHIR
- Patient Records
- HL7
trust_url: https://www.healthgorilla.com/home/company/health-data-security
---
