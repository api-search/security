---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:mk@tripfix.de"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tripfix.de
  spf: true
hosts:
- cert_expires: Dec 23 08:06:21 2026 GMT
  host: tripfix.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tripfix De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tripfix-de, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: tripfix-de
provider_slug: tripfix-de
slug: tripfix-de-domain-security
source_filename: tripfix-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tripfix.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 08:06:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tripfix.de\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:mk@tripfix.de\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tripfix-de/security/tripfix-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Expense
- SaaS
- Germany
- Freelancers
---
