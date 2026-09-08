---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: advancechip.com
  probed_hosts_without_tls:
  - advancechip.com
  - en.advancechip.com
  spf: true
  tls_cert_expired: '2023-01-13'
  tls_cert_subject: C=XX, L=Default City, O=Default Company Ltd
hosts:
- host: www.advancechip.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Advancechip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advancechip Technology (Hunan) Co., Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Advancechip Technology (Hunan) Co., Ltd.
provider_slug: advancechip
slug: advancechip-domain-security
source_filename: advancechip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  HTTPS is offered in name only. Port 443 on www.advancechip.com (180.76.137.252) answers with a\n  default placeholder certificate — subject and issuer both \"C=XX, L=Default City, O=Default Company\n  Ltd\", RSA 2048 / sha256WithRSAEncryption — issued 2022-01-13 and EXPIRED 2023-01-13, matching no\n  Advancechip hostname. advancechip.com and en.advancechip.com fail the TLS handshake outright\n  (SSLV3_ALERT_HANDSHAKE_FAILURE). Every page of the corporate site, including the download and\n  contact forms, is therefore served over plaintext HTTP, and robots.txt advertises both sitemaps\n  over http. No HSTS on any host. Email is better defended than the web tier: SPF is published and\n  DMARC is at p=reject, but the zone is not DNSSEC-signed and publishes no CAA record.\nhosts:\n- host: www.advancechip.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED]\
  \ certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: advancechip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  tls_cert_subject: C=XX, L=Default City, O=Default Company Ltd\n  tls_cert_expired: '2023-01-13'\n  probed_hosts_without_tls:\n  - advancechip.com\n  - en.advancechip.com\nchecked: '2026-09-07'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advancechip/refs/heads/main/security/advancechip-domain-security.yml
summary_line: DMARC
tags:
- Company
- Semiconductors
- Integrated Circuits
- Digital Signal Processing
- Embedded Systems
- System On Chip
- Automotive Electronics
- Motor Control
- Industrial Control
- Hardware
- China
---
