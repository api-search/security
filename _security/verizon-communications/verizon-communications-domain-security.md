---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: verizon-communications.com
  spf: false
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verizon.com
  spf: true
hosts:
- host: www.verizon-communications.com
  https: false
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: developers.verizon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.verizon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verizon Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verizon Communications, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Verizon Communications
provider_slug: verizon-communications
slug: verizon-communications-domain-security
source_filename: verizon-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verizon-communications.com\n  https: false\n- host: developers.verizon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.verizon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: verizon-communications.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: verizon.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verizon-communications/refs/heads/main/security/verizon-communications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Wireless
- Network APIs
- IoT
- 5G
- Enterprise
- Identity
- Fortune 100
---
