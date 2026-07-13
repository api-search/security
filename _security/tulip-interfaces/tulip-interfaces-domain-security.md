---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tulip.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tulip.com
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: tulip.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 13:13:50 2026 GMT
  host: docs.tulip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 01:15:59 2026 GMT
  host: support.tulip.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tulip Interfaces Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tulip Interfaces, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tulip Interfaces
provider_slug: tulip-interfaces
slug: tulip-interfaces-domain-security
source_filename: tulip-interfaces-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tulip.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\n- host: docs.tulip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 13:13:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.tulip.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 01:15:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tulip.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tulip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tulip-interfaces/refs/heads/main/security/tulip-interfaces-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Manufacturing
- MES
- Industrial IoT
- Shop Floor
- Low-Code
- Frontline Operations
---
