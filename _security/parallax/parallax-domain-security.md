---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: withparallax.com
  spf: false
hosts:
- cert_expires: Oct 14 07:04:02 2026 GMT
  host: www.withparallax.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parallax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parallax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Parallax
provider_slug: parallax
slug: parallax-domain-security
source_filename: parallax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.withparallax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:04:02 2026 GMT\n  hsts: null\ndomains:\n- domain: withparallax.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallax/refs/heads/main/security/parallax-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Payments
- Cross-Border Payments
- Stablecoins
- Crypto
- Fintech
- Remittances
- B2B Payments
---
