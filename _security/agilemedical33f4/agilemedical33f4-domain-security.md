---
description: ''
domains:
- a:
  - 121.41.170.158
  caa: []
  dmarc: false
  dnssec: false
  domain: agibot.cn
  ns:
  - dns15.hichina.com
  - dns16.hichina.com
  spf: true
hosts:
- alt_svc: h3
  cert_issuer: Let's Encrypt (CN=YR2)
  cert_not_after: '2026-11-05'
  cert_not_before: '2026-08-07'
  cert_subject: CN=www.agibot.cn
  host: www.agibot.cn
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  hsts_preload: false
  http_status: 200
  http_version: h2
  https: true
  server: nginx
  tls_version: TLSv1.3
- host: agibot.cn
  http_status: 200
  https: true
  note: apex serves the same site as www
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Agilemedical33F4 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agile Medical, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agile Medical
provider_slug: agilemedical33f4
slug: agilemedical33f4-domain-security
source_filename: agilemedical33f4-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the apis.yml Website host (www.agibot.cn) and its apex\nnote: >-\n  The mechanical probe (0-working/probe-domain-security.py) recorded https:false for www.agibot.cn,\n  which is a false negative — the origin in Suzhou is slow and intermittently drops non-browser\n  requests from this vantage point. Re-probed by hand with curl and openssl s_client: the host\n  serves HTTP/2 over TLSv1.3 with HSTS. The values below are the observed ones.\nhosts:\n- host: www.agibot.cn\n  https: true\n  http_status: 200\n  http_version: h2\n  tls_version: TLSv1.3\n  cert_issuer: \"Let's Encrypt (CN=YR2)\"\n  cert_subject: CN=www.agibot.cn\n  cert_not_before: '2026-08-07'\n  cert_not_after: '2026-11-05'\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  hsts_preload: false\n  server: nginx\n  alt_svc: h3\n- host: agibot.cn\n  https: true\n  http_status: 200\n  note: apex serves the same site as\
  \ www\ndomains:\n- domain: agibot.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  ns: [dns15.hichina.com, dns16.hichina.com]\n  a: [121.41.170.158]\nx-evidence:\n  fetched: '2026-09-12'\n  probes:\n  - {url: 'https://www.agibot.cn/', method: HEAD, status: 200}\n  - {url: 'https://agibot.cn/', method: GET, status: 200}\n  - {check: tls, host: www.agibot.cn, result: TLSv1.3}\n  - {check: hsts, host: www.agibot.cn, header: 'strict-transport-security: max-age=31536000'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agilemedical33f4/refs/heads/main/security/agilemedical33f4-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Surgical Robotics
- Medical Devices
- Robotics
- Healthcare
- Minimally Invasive Surgery
- Medical Imaging
- Artificial Intelligence
- China
---
