---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  dmarc: false
  dnssec: false
  domain: baania.com
  spf: true
hosts:
- cert_expires: Oct  4 05:56:53 2026 GMT
  host: baania.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baania Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baania, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Baania
provider_slug: baania
slug: baania-domain-security
source_filename: baania-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baania.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:56:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: baania.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baania/refs/heads/main/security/baania-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Real Estate
- Proptech
- Property
- Marketplace
- Thailand
---
