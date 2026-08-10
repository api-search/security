---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: atera.com
  spf: true
hosts:
- cert_expires: Oct 18 12:25:09 2026 GMT
  host: www.atera.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 11:30:57 2026 GMT
  host: app.atera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atera, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Atera
provider_slug: atera
slug: atera-domain-security
source_filename: atera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 12:25:09 2026 GMT\n  hsts: null\n- host: app.atera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 11:30:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atera.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atera/refs/heads/main/security/atera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- IT Management
- RMM
- PSA
- Helpdesk
- Ticketing
- Patch Management
- Remote Monitoring
- Endpoint Management
- MSP
- Network Discovery
- Alerts
- Devices
- Billing
- Webhooks
- AI
---
