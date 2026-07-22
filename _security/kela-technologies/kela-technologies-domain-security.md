---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kela.io
  spf: false
hosts:
- cert_expires: Sep  6 22:10:18 2026 GMT
  host: kela.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kela Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kela Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kela Technologies
provider_slug: kela-technologies
slug: kela-technologies-domain-security
source_filename: kela-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kela.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:10:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: kela.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kela-technologies/refs/heads/main/security/kela-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Defense
- Defense Technology
- Military
- Systems Integration
- Space
- Satellite
- National Security
---
