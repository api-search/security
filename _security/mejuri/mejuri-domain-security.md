---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mejuri.com
  spf: true
hosts:
- cert_expires: Sep 28 02:12:02 2026 GMT
  host: mejuri.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mejuri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mejuri, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mejuri
provider_slug: mejuri
slug: mejuri-domain-security
source_filename: mejuri-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mejuri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 02:12:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mejuri.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mejuri/refs/heads/main/security/mejuri-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Jewelry
- Fashion
- Retail
- E-Commerce
- Direct-to-Consumer
- Consumer Brand
---
