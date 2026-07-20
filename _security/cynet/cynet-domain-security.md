---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cynet.com
  spf: true
hosts:
- cert_expires: Sep 27 16:27:09 2026 GMT
  host: cynet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 14:07:39 2026 GMT
  host: portal.cynet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 01:50:14 2026 GMT
  host: help.api.cynet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cynet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cynet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cynet
provider_slug: cynet
slug: cynet-domain-security
source_filename: cynet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cynet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:27:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.cynet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:07:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.api.cynet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:50:14 2026 GMT\n  hsts: null\ndomains:\n- domain: cynet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cynet/refs/heads/main/security/cynet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Security
- XDR
- EDR
- MDR
- SOAR
- Endpoint Security
- Threat Detection
- Incident Response
- MSP
---
