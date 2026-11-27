---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: miraqo.io
  spf: true
hosts:
- cert_expires: Dec 22 19:15:58 2026 GMT
  host: miraqo.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Miraqo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Miraqo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Miraqo
provider_slug: miraqo-io
slug: miraqo-io-domain-security
source_filename: miraqo-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: miraqo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 19:15:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: miraqo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/miraqo-io/security/miraqo-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SEO
- Marketing
- Software-as-a-Service
- Freelancers
- Agencies
---
