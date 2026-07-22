---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: born.com
  spf: true
hosts:
- cert_expires: Aug 20 19:37:49 2026 GMT
  host: www.born.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Born Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Born, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Born
provider_slug: born
slug: born-domain-security
source_filename: born-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.born.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 19:37:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: born.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/born/refs/heads/main/security/born-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Artificial Intelligence
- AI Companions
- Mobile Apps
- Social
- Gaming
---
