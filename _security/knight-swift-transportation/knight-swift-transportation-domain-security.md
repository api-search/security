---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: knight-swift.com
  spf: true
hosts:
- cert_expires: Sep 25 20:38:26 2026 GMT
  host: www.knight-swift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.knight-swift.com
  https: false
- host: api.knight-swift.com
  https: false
kind: domain-security
layout: security
method: probed
name: Knight Swift Transportation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knight-Swift Transportation, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Knight-Swift Transportation
provider_slug: knight-swift-transportation
slug: knight-swift-transportation-domain-security
source_filename: knight-swift-transportation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.knight-swift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:38:26 2026 GMT\n  hsts: false\n- host: developer.knight-swift.com\n  https: false\n- host: api.knight-swift.com\n  https: false\ndomains:\n- domain: knight-swift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knight-swift-transportation/refs/heads/main/security/knight-swift-transportation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Trucking
- Transportation
- Logistics
---
