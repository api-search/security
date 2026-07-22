---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lynqnetworks.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: lynqnetworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lynq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lynq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lynq
provider_slug: lynq
slug: lynq-domain-security
source_filename: lynq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lynqnetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lynqnetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lynq/refs/heads/main/security/lynq-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Wireless
- Networking
- Connectivity
- IoT
- Hardware
- OEM
---
