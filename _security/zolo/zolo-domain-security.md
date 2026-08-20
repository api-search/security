---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "  pki.goog"
  - 0 issuewild " digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zolo.ca
  spf: true
hosts:
- cert_expires: Oct  3 16:44:40 2026 GMT
  host: www.zolo.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zolo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zolo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zolo
provider_slug: zolo
slug: zolo-domain-security
source_filename: zolo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zolo.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:44:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zolo.ca\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"  pki.goog\"\n  - 0 issuewild \" digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zolo/refs/heads/main/security/zolo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- Canada
- Property Listings
- MLS
- IDX
- Valuation
- AVM
- PropTech
- Rentals
- Mortgage
- Conveyancing
---
