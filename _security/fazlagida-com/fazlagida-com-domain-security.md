---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fazlagida.com
  spf: true
hosts:
- cert_expires: Dec  7 10:36:13 2026 GMT
  host: fazlagida.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fazlagida Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fazla Gida, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fazla Gida
provider_slug: fazlagida-com
slug: fazlagida-com-domain-security
source_filename: fazlagida-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fazlagida.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 10:36:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fazlagida.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fazlagida-com/security/fazlagida-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Waste Management
- Food Waste
- Circular Economy
- Sustainability Consultancy
- Animal Feed
- Recycling
- Donation
---
