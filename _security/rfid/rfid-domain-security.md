---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zebra.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: clearstreamrfid.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: developer.zebra.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 20:44:47 2026 GMT
  host: www.clearstreamrfid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: www.gs1.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rfid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RFID, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RFID
provider_slug: rfid
slug: rfid-domain-security
source_filename: rfid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.zebra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\n- host: www.clearstreamrfid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:44:47 2026 GMT\n  hsts: false\n- host: www.gs1.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zebra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: clearstreamrfid.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rfid/refs/heads/main/security/rfid-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- RFID
- IoT
- Supply Chain
- Inventory Management
- Asset Tracking
- GS1
- EPCIS
---
