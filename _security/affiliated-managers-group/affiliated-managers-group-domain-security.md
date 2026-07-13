---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amg.com
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: www.amg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: wealth.amg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Affiliated Managers Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affiliated Managers Group, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Affiliated Managers Group
provider_slug: affiliated-managers-group
slug: affiliated-managers-group-domain-security
source_filename: affiliated-managers-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wealth.amg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affiliated-managers-group/refs/heads/main/security/affiliated-managers-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Asset Management
- Investment Management
- Financial Services
- Wealth Management
- Institutional Investing
- Fortune 1000
---
