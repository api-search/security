---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: argussoftware.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: altusgroup.com
  spf: true
hosts:
- host: www.argussoftware.com
  https: false
- cert_expires: Sep  1 17:18:54 2026 GMT
  host: www.altusgroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Argus Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argus Software, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Argus Software
provider_slug: argus-software
slug: argus-software-domain-security
source_filename: argus-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.argussoftware.com\n  https: false\n- host: www.altusgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:18:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: argussoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: altusgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argus-software/refs/heads/main/security/argus-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Commercial Real Estate
- PropTech
- Valuation
- Asset Management
- Investment Management
- Software
---
