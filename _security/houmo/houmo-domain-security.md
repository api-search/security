---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: houmoai.com
  spf: false
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: www.houmoai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Houmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for houmo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: houmo
provider_slug: houmo
slug: houmo-domain-security
source_filename: houmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.houmoai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: houmoai.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/houmo/refs/heads/main/security/houmo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Semiconductors
- AI Chips
- Edge Computing
- Compute In Memory
- Machine Learning
- Hardware
---
