---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: b2b-center.ru
  spf: true
hosts:
- cert_expires: Jan 24 10:44:47 2027 GMT
  host: www.b2b-center.ru
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: B2B Center Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for B2B-Center, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: B2B-Center
provider_slug: b2b-center
slug: b2b-center-domain-security
source_filename: b2b-center-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.b2b-center.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 10:44:47 2027 GMT\n  hsts: null\ndomains:\n- domain: b2b-center.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b2b-center/refs/heads/main/security/b2b-center-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Procurement
- E-Procurement
- Marketplace
- B2B
- Trading Platform
- Sourcing
- Russia
---
