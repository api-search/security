---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: encorehq.co
  spf: false
hosts:
- cert_expires: Dec 14 11:13:06 2026 GMT
  host: encorehq.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Encorehq Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for encorehq-co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: encorehq-co
provider_slug: encorehq-co
slug: encorehq-co-domain-security
source_filename: encorehq-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: encorehq.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 11:13:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: encorehq.co\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/encorehq-co/security/encorehq-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Feedback
- Design
- Product
- SaaS
---
