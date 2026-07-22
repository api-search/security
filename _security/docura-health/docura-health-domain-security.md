---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: docurahealth.com
  spf: true
hosts:
- cert_expires: Sep 25 03:48:48 2026 GMT
  host: www.docurahealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docura Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docura Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Docura Health
provider_slug: docura-health
slug: docura-health-domain-security
source_filename: docura-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docurahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 03:48:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: docurahealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docura-health/refs/heads/main/security/docura-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health
- Medical-Legal
- Medical Records
- Impairment Rating
- IME
- QME
- Workers Compensation
- HIPAA
- Clinical Documentation
---
