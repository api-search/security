---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: pops.fyi
  spf: false
hosts:
- cert_expires: Oct 18 18:03:25 2026 GMT
  host: pops.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pops, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Pops
provider_slug: pops
slug: pops-domain-security
source_filename: pops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pops.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 18:03:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pops.fyi\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pops/refs/heads/main/security/pops-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Gaming
- Social
- Artificial Intelligence
- Mobile
- Entertainment
---
