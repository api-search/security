---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acehardware.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acehardware-vendors.com
  spf: false
hosts:
- cert_expires: Aug 16 11:30:44 2026 GMT
  host: www.acehardware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: www.acehardware-vendors.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ace Hardware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ace Hardware, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ace Hardware
provider_slug: ace-hardware
slug: ace-hardware-domain-security
source_filename: ace-hardware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acehardware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 11:30:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.acehardware-vendors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: acehardware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: acehardware-vendors.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ace-hardware/refs/heads/main/security/ace-hardware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Hardware
- Home Improvement
- Tools
- Paint
- Cooperative
- EDI
- Affiliate
---
