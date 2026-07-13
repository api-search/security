---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zebra.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.zebra.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: developer.zebra.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: api.zebra.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zebra Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zebra Technologies, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zebra Technologies
provider_slug: zebra-technologies
slug: zebra-technologies-domain-security
source_filename: zebra-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zebra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.zebra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\n- host: api.zebra.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zebra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zebra-technologies/refs/heads/main/security/zebra-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Manufacturing
- RFID
- Barcode
- Warehouse Automation
- IoT
- Industrial IoT
- Fortune 500
---
