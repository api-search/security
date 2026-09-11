---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: footlocker.com
  spf: true
hosts:
- cert_expires: Oct 21 02:38:22 2026 GMT
  host: www.footlocker.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foot Locker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foot Locker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Foot Locker
provider_slug: foot-locker
slug: foot-locker-domain-security
source_filename: foot-locker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.footlocker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 02:38:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: footlocker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foot-locker/refs/heads/main/security/foot-locker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Retail
- Footwear
- Apparel
- E-Commerce
- Sneakers
- Omnichannel
---
