---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sequans.com
  spf: true
hosts:
- cert_expires: Oct 31 22:27:04 2026 GMT
  host: sequans.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sequans Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sequans, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sequans
provider_slug: sequans
slug: sequans-domain-security
source_filename: sequans-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sequans.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 22:27:04 2026 GMT\n  hsts: false\ndomains:\n- domain: sequans.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequans/refs/heads/main/security/sequans-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semiconductors
- Cellular IoT
- 5G
- LTE-M
- NB-IoT
- IoT Modules
- Hardware
- Telecommunications
- France
---
