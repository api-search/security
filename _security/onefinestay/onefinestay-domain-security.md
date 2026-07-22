---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: onefinestay.com
  spf: true
hosts:
- cert_expires: Sep 20 01:27:48 2026 GMT
  host: www.onefinestay.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onefinestay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onefinestay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Onefinestay
provider_slug: onefinestay
slug: onefinestay-domain-security
source_filename: onefinestay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onefinestay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:27:48 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: onefinestay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onefinestay/refs/heads/main/security/onefinestay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Hospitality
- Travel
- Vacation Rentals
- Luxury
- Accommodation
- Real Estate
---
