---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: penguindriver.com
  spf: false
hosts:
- cert_expires: Jan 24 10:13:15 2027 GMT
  host: penguindriver.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Penguindriver Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for penguindriver-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: penguindriver-com
provider_slug: penguindriver-com
slug: penguindriver-com-domain-security
source_filename: penguindriver-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: penguindriver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 10:13:15 2027 GMT\n  hsts: false\ndomains:\n- domain: penguindriver.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/penguindriver-com/security/penguindriver-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Taiwan
- Aggregator
- Data
---
