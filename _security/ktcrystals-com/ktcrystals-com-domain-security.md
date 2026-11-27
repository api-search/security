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
  domain: ktcrystals.com
  spf: true
hosts:
- cert_expires: Feb  5 08:31:09 2027 GMT
  host: ktcrystals.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KT Crystals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KT Crystals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KT Crystals
provider_slug: ktcrystals-com
slug: ktcrystals-com-domain-security
source_filename: ktcrystals-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ktcrystals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 08:31:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ktcrystals.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ktcrystals-com/security/ktcrystals-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wholesale
- Crystal
- Jewelry
- Supplier
- Retail
---
