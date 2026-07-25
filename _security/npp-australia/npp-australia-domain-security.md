---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: auspayplus.com.au
  spf: true
hosts:
- cert_expires: Oct 17 17:10:00 2026 GMT
  host: www.auspayplus.com.au
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Npp Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NPP Australia (AP+), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NPP Australia (AP+)
provider_slug: npp-australia
slug: npp-australia-domain-security
source_filename: npp-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.auspayplus.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 17:10:00 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: auspayplus.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/npp-australia/refs/heads/main/security/npp-australia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- Real-Time Payments
- Account-to-Account
- ISO 20022
- Payment Scheme
- Rails
- PayTo
- PayID
- Open Banking
---
