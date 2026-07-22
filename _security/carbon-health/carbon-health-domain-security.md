---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: carbonhealth.com
  spf: true
hosts:
- cert_expires: Oct 10 22:47:56 2026 GMT
  host: carbonhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carbon Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbon Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Carbon Health
provider_slug: carbon-health
slug: carbon-health-domain-security
source_filename: carbon-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carbonhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 22:47:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carbonhealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbon-health/refs/heads/main/security/carbon-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Telemedicine
- Urgent Care
- Primary Care
- Digital Health
- Clinical Research
---
