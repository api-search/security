---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: corenaturalresources.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: archresources.com
  legacy: true
  spf: false
- domain: arch-coal.com
  legacy: true
  resolves: false
hosts:
- cert_expires: Oct 12 05:02:30 2026 GMT
  cert_issuer: Let's Encrypt
  host: corenaturalresources.com
  hsts: false
  http_status: 200
  https: true
  server: Apache
- host: www.corenaturalresources.com
  http_status: 301
  https: true
  redirects_to: https://corenaturalresources.com/
- cert_expires: Sep 27 13:42:12 2026 GMT
  cert_issuer: Google Trust Services
  host: investors.corenaturalresources.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  server: cloudflare
  x_frame_options: SAMEORIGIN
- host: archresources.com
  http_status: 200
  https: true
  legacy: true
- host: www.arch-coal.com
  https: false
  legacy: true
  resolves: false
kind: domain-security
layout: security
method: probed
name: Arch Coal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arch Coal, probed live across 5 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS; 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Arch Coal
provider_slug: arch-coal
slug: arch-coal-domain-security
source_filename: arch-coal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the corenaturalresources.com properties in apis.yml\nnotes: Arch Coal / Arch Resources is now Core Natural Resources (NYSE:CNR) following the January\n  2025 merger with CONSOL Energy. The arch-coal.com domain no longer resolves. archresources.com\n  still answers but the corporate presence has moved to corenaturalresources.com.\nhosts:\n- host: corenaturalresources.com\n  https: true\n  http_status: 200\n  server: Apache\n  cert_issuer: Let's Encrypt\n  cert_expires: Oct 12 05:02:30 2026 GMT\n  hsts: false\n- host: www.corenaturalresources.com\n  https: true\n  http_status: 301\n  redirects_to: https://corenaturalresources.com/\n- host: investors.corenaturalresources.com\n  https: true\n  http_status: 200\n  server: cloudflare\n  cert_issuer: Google Trust Services\n  cert_expires: Sep 27 13:42:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  x_frame_options:\
  \ SAMEORIGIN\n- host: archresources.com\n  https: true\n  http_status: 200\n  legacy: true\n- host: www.arch-coal.com\n  https: false\n  resolves: false\n  legacy: true\ndomains:\n- domain: corenaturalresources.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: archresources.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n  legacy: true\n- domain: arch-coal.com\n  resolves: false\n  legacy: true\nfindings:\n- severity: medium\n  finding: The primary corporate domain corenaturalresources.com publishes no SPF and no DMARC\n    record, leaving the merged company's domain open to email spoofing. The legacy archresources.com\n    domain still has DMARC at p=reject.\n- severity: low\n  finding: No CAA records and no DNSSEC on corenaturalresources.com.\n- severity: low\n  finding: The corporate site does not send HSTS; the investor relations portal does.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/security/arch-coal-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Mining
- Coal
- Metallurgical Coal
- Thermal Coal
- Energy
- Core Natural Resources
- Investor Relations
- Fortune 500
---
