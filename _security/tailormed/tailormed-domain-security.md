---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tailormed.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tailormed.co
  spf: true
hosts:
- cert_expires: Nov 15 17:38:27 2026 GMT
  host: www.tailormed.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 14:38:37 2026 GMT
  host: hub.tailormed.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 11:31:13 2026 GMT
  host: auth.tailormed.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tailormed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TailorMed, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TailorMed
provider_slug: tailormed
slug: tailormed-domain-security
source_filename: tailormed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tailormed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 17:38:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: hub.tailormed.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 14:38:37 2026 GMT\n  hsts: false\n- host: auth.tailormed.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 11:31:13 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\ndomains:\n- domain: tailormed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tailormed.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailormed/refs/heads/main/security/tailormed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health IT
- Medication Access
- Medication Affordability
- Financial Navigation
- Patient Assistance
- Pharmacy
- Oncology
- Revenue Cycle
- HL7
- FHIR
- Life Sciences
---
