---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: firstam.com
  spf: true
hosts:
- cert_expires: Sep 18 19:38:18 2026 GMT
  host: www.firstam.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: developer.firstam.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: First American Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First American Financial, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: First American Financial
provider_slug: first-american-financial
slug: first-american-financial-domain-security
source_filename: first-american-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firstam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 19:38:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.firstam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: firstam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/security/first-american-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Title Insurance
- Real Estate
- Settlement Services
- Financial Services
- Fortune 1000
---
