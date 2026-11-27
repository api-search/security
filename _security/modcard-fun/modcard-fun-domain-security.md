---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: modcard.fun
  spf: true
hosts:
- cert_expires: Feb 11 22:32:44 2027 GMT
  host: modcard.fun
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ModCard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ModCard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ModCard
provider_slug: modcard-fun
slug: modcard-fun-domain-security
source_filename: modcard-fun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modcard.fun\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 22:32:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: modcard.fun\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/modcard-fun/security/modcard-fun-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E‑cards
- Personalized
- Greeting Cards
- Digital Gifts
---
