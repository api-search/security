---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: diamondstandard.co
  spf: true
hosts:
- cert_expires: Dec 21 13:21:41 2026 GMT
  host: www.diamondstandard.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Diamondstandard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diamondstandard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Diamondstandard
provider_slug: diamondstandard
slug: diamondstandard-domain-security
source_filename: diamondstandard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.diamondstandard.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 13:21:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: diamondstandard.co\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/diamondstandard/security/diamondstandard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Investment
- Blockchain
- Commodities
---
