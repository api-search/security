---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: skyfri.com
  spf: true
hosts:
- cert_expires: Sep 13 01:29:20 2026 GMT
  host: www.skyfri.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skyfri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skyfri, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Skyfri
provider_slug: skyfri
slug: skyfri-domain-security
source_filename: skyfri-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skyfri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 01:29:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: skyfri.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyfri/refs/heads/main/security/skyfri-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Solar
- Energy
- Cleantech
- Renewable Energy
- Asset Management
- SCADA
- Monitoring
- IoT
---
