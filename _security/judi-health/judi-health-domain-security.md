---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: judi.health
  spf: false
hosts:
- cert_expires: Aug 27 15:41:36 2026 GMT
  host: www.judi.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Judi Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Judi Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Judi Health
provider_slug: judi-health
slug: judi-health-domain-security
source_filename: judi-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.judi.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 15:41:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: judi.health\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/judi-health/refs/heads/main/security/judi-health-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Pharmacy Benefits
- PBM
- Health Benefits
- Benefits Administration
- Health Technology
- Medicare
- Insurance
---
