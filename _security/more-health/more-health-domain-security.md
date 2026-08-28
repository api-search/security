---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: morehealth.com
  spf: true
hosts:
- cert_expires: Nov 19 17:59:17 2026 GMT
  host: morehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: More Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MORE Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MORE Health
provider_slug: more-health
slug: more-health-domain-security
source_filename: more-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: morehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 17:59:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: morehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/more-health/refs/heads/main/security/more-health-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Healthcare
- Digital Health
- Telemedicine
- Telehealth
- Second Opinion
- Medical Records
- Care Coordination
- Employee Benefits
- HIPAA
- Cross-Border Care
---
