---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kittl.com
  spf: true
hosts:
- cert_expires: Sep 14 10:42:44 2026 GMT
  host: www.kittl.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kittl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kittl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kittl
provider_slug: kittl
slug: kittl-domain-security
source_filename: kittl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kittl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 10:42:44 2026 GMT\n  hsts: false\ndomains:\n- domain: kittl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kittl/refs/heads/main/security/kittl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Design
- Graphic Design
- Creative Tools
- SDK
- Developer Platform
- Extensions
- Print On Demand
- E-Commerce
- AI
- Mockups
- Typography
---
