---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: craftingstepbystep.com
  spf: true
hosts:
- cert_expires: Jan 14 15:05:54 2027 GMT
  host: www.craftingstepbystep.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crafting Step by Step Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crafting Step by Step, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crafting Step by Step
provider_slug: craftingstepbystep-com
slug: craftingstepbystep-com-domain-security
source_filename: craftingstepbystep-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.craftingstepbystep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 15:05:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: craftingstepbystep.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/craftingstepbystep-com/security/craftingstepbystep-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crafts
- Tutorials
- How-To
- DIY
- Education
- MCP
---
