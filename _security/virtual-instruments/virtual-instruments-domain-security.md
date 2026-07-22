---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: virtana.com
  spf: true
hosts:
- cert_expires: Sep 15 13:55:28 2026 GMT
  host: www.virtana.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: docs.virtana.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: app.cloud.virtana.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Virtual Instruments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virtana (Virtual Instruments), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Virtana (Virtual Instruments)
provider_slug: virtual-instruments
slug: virtual-instruments-domain-security
source_filename: virtual-instruments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.virtana.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 13:55:28 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: docs.virtana.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: false\n- host: app.cloud.virtana.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: virtana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtual-instruments/refs/heads/main/security/virtual-instruments-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Observability
- Monitoring
- Storage
- Cloud Cost Management
- AIOps
- Performance
- Alerts
- MCP
---
