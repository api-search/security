---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: covetrus.com
  spf: true
hosts:
- cert_expires: Dec 10 14:37:14 2026 GMT
  host: covetrus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Covetrus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Covetrus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Covetrus
provider_slug: covetrus
slug: covetrus-domain-security
source_filename: covetrus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: covetrus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 14:37:14 2026 GMT\n  hsts: false\ndomains:\n- domain: covetrus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/covetrus/security/covetrus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Veterinary
- Software
- Pharmacy
- Client-Communication
---
