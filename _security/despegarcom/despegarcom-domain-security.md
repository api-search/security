---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: despegar.com
  spf: true
hosts:
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.despegar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Despegarcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Despegar.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Despegar.com
provider_slug: despegarcom
slug: despegarcom-domain-security
source_filename: despegarcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.despegar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: despegar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/despegarcom/refs/heads/main/security/despegarcom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Travel
- Hotels
- Flights
- Activities
- Booking
- Latin America
- B2B
- MCP
- Webhooks
---
