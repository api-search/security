---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: warbyparker.com
  spf: true
hosts:
- cert_expires: Oct 13 14:58:00 2026 GMT
  host: www.warbyparker.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Warby Parker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Warby Parker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Warby Parker
provider_slug: warby-parker
slug: warby-parker-domain-security
source_filename: warby-parker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.warbyparker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 14:58:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: warbyparker.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warby-parker/refs/heads/main/security/warby-parker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Eyewear
- Retail
- E-commerce
- Vision Care
- Optical
- Direct-to-Consumer
---
