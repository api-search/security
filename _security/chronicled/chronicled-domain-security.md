---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chronicled.com
  spf: false
hosts:
- cert_expires: Sep 25 13:41:55 2026 GMT
  host: www.chronicled.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chronicled Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chronicled, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Chronicled
provider_slug: chronicled
slug: chronicled-domain-security
source_filename: chronicled-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chronicled.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:41:55 2026 GMT\n  hsts: false\ndomains:\n- domain: chronicled.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chronicled/refs/heads/main/security/chronicled-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Crypto
- Blockchain
- Supply Chain
- Pharmaceutical
- Life Sciences
- Healthcare
- DSCSA
- Compliance
---
