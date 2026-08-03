---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ambiencehealthcare.com
  spf: true
hosts:
- cert_expires: Oct 21 03:50:54 2026 GMT
  host: www.ambiencehealthcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 16:57:22 2026 GMT
  host: docs.ambiencehealthcare.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 06:51:48 2026 GMT
  host: auth.ambiencehealthcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ambience Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambience Healthcare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ambience Healthcare
provider_slug: ambience-healthcare
slug: ambience-healthcare-domain-security
source_filename: ambience-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ambiencehealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 03:50:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ambiencehealthcare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 16:57:22 2026 GMT\n  hsts: false\n- host: auth.ambiencehealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 06:51:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ambiencehealthcare.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambience-healthcare/refs/heads/main/security/ambience-healthcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- Clinical Documentation
- Ambient AI
- Medical Coding
- Electronic Health Records
- FHIR
- Health IT
- Speech Recognition
---
