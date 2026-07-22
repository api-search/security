---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vendorpm.com
  spf: true
hosts:
- cert_expires: Sep 12 04:34:41 2026 GMT
  host: vendorpm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vendorpm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VendorPM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VendorPM
provider_slug: vendorpm
slug: vendorpm-domain-security
source_filename: vendorpm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vendorpm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:34:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vendorpm.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendorpm/refs/heads/main/security/vendorpm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Vertical Software
- PropTech
- Procurement
- Real Estate
- Property Management
- Vendor Management
- Contract Management
- Compliance
---
