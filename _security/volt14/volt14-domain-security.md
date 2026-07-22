---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: volt14.com
  spf: true
hosts:
- cert_expires: Dec 14 00:46:08 2026 GMT
  host: volt14.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Volt14 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volt14, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Volt14
provider_slug: volt14
slug: volt14-domain-security
source_filename: volt14-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: volt14.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 14 00:46:08 2026 GMT\n  hsts: false\ndomains:\n- domain: volt14.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volt14/refs/heads/main/security/volt14-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Batteries
- Energy Storage
- Materials Science
- Lithium-Ion
- Anode Technology
- Deep Tech
- Electric Vehicles
---
