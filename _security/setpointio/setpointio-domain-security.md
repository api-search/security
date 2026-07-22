---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: setpoint.io
  spf: true
hosts:
- cert_expires: Oct  1 06:45:12 2026 GMT
  host: setpoint.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Setpointio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Setpoint.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Setpoint.io
provider_slug: setpointio
slug: setpointio-domain-security
source_filename: setpointio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: setpoint.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:45:12 2026 GMT\n  hsts: false\ndomains:\n- domain: setpoint.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/setpointio/refs/heads/main/security/setpointio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Capital Markets
- Asset-Backed Finance
- Debt Capital
- Securitization
- Warehouse Lending
- Financial Services
---
