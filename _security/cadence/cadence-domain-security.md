---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cadence.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eyesopen.com
  spf: true
hosts:
- cert_expires: Nov 26 16:29:33 2026 GMT
  host: www.cadence.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 24 20:34:49 2026 GMT
  host: www.eyesopen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: orion.eyesopen.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cadence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cadence Design Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cadence Design Systems
provider_slug: cadence
slug: cadence-domain-security
source_filename: cadence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cadence.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 16:29:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.eyesopen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 20:34:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: orion.eyesopen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: cadence.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: eyesopen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cadence/refs/heads/main/security/cadence-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Electronic Design Automation
- EDA
- Semiconductors
- Chip Design
- IC Design
- PCB Design
- Software
- Company
---
