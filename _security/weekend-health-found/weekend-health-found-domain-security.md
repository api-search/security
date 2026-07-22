---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: weekendhealth.com
  spf: true
hosts:
- cert_expires: Oct  1 18:15:03 2026 GMT
  host: www.weekendhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weekend Health Found Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weekend Health (Found), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Weekend Health (Found)
provider_slug: weekend-health-found
slug: weekend-health-found-domain-security
source_filename: weekend-health-found-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weekendhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:15:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: weekendhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weekend-health-found/refs/heads/main/security/weekend-health-found-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Healthcare
- Telehealth
- Weight Loss
- GLP-1
- Digital Health
---
