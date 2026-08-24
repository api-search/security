---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kromatid.com
  spf: true
hosts:
- cert_expires: Oct 23 02:23:12 2026 GMT
  host: kromatid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kromatid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KromaTiD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KromaTiD
provider_slug: kromatid
slug: kromatid-domain-security
source_filename: kromatid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kromatid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 02:23:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kromatid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kromatid/refs/heads/main/security/kromatid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Genomics
- Biotechnology
- Life Sciences
- Cell and Gene Therapy
- Cytogenetics
- Laboratory Services
- Healthcare
- Research
---
