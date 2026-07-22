---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hashboard.com
  spf: false
hosts:
- cert_expires: Sep 10 00:17:09 2026 GMT
  host: hashboard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hashboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hashboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Hashboard
provider_slug: hashboard
slug: hashboard-domain-security
source_filename: hashboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hashboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 00:17:09 2026 GMT\n  hsts: false\ndomains:\n- domain: hashboard.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hashboard/refs/heads/main/security/hashboard-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- B2B
- Business Intelligence
- Analytics
- Data
- BI-as-Code
- Dashboards
- Data Visualization
- Developer Tools
- CLI
---
