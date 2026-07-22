---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: alaffiahealth.com
  spf: true
hosts:
- cert_expires: Oct 15 04:50:59 2026 GMT
  host: alaffiahealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alaffia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alaffia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Alaffia
provider_slug: alaffia
slug: alaffia-domain-security
source_filename: alaffia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alaffiahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 04:50:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alaffiahealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alaffia/refs/heads/main/security/alaffia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health Insurance
- Payment Integrity
- Claims
- Utilization Management
- Artificial Intelligence
- Machine Learning
- Insurtech
- Healthtech
- United States
---
