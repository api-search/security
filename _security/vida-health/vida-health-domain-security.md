---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: vida.com
  spf: true
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: www.vida.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  3 01:36:31 2026 GMT
  host: api.vida.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: live API host; returns HTTP 401 on every probed path (no anonymous surface)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vida Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vida Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Vida Health
provider_slug: vida-health
slug: vida-health-domain-security
source_filename: vida-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vida.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.vida.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 01:36:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: live API host; returns HTTP 401 on every probed path (no anonymous surface)\ndomains:\n- domain: vida.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vida-health/refs/heads/main/security/vida-health-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Health
- Virtual Care
- Chronic Care
- Behavioral Health
- Telehealth
- Employee Benefits
- Health Plans
---
