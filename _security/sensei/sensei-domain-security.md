---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sensei.tech
  spf: true
hosts:
- cert_expires: Sep 25 00:38:23 2026 GMT
  host: sensei.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sensei Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sensei, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Sensei
provider_slug: sensei
slug: sensei-domain-security
source_filename: sensei-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sensei.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:38:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sensei.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensei/refs/heads/main/security/sensei-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Autonomous Retail
- Computer Vision
- Artificial Intelligence
- Retail Technology
- Checkout-Free
- Frictionless Shopping
---
