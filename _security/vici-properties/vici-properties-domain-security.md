---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: viciproperties.com
  spf: true
hosts:
- cert_expires: Sep  5 05:51:28 2026 GMT
  host: www.viciproperties.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vici Properties Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VICI Properties, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VICI Properties
provider_slug: vici-properties
slug: vici-properties-domain-security
source_filename: vici-properties-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.viciproperties.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:51:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: viciproperties.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vici-properties/refs/heads/main/security/vici-properties-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Casinos
- Experiential Real Estate
- Gaming
- Hospitality
- Real Estate
- REIT
---
