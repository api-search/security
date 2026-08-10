---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: minthouse.com
  spf: true
hosts:
- cert_expires: Oct 22 09:07:19 2026 GMT
  host: minthouse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mint House Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mint House, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mint House
provider_slug: mint-house
slug: mint-house-domain-security
source_filename: mint-house-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: minthouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 09:07:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: minthouse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mint-house/refs/heads/main/security/mint-house-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hospitality
- Travel
- Lodging
- Apartment Hotels
- Short Term Rental
- Real Estate
- Property Management
---
