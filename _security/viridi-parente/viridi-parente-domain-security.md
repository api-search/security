---
api_specs:
- filename: viridi-parente-vista-openapi.json
  format: json
  label: Viridi ViSTA Platform API
  slug: viridi-parente-vista
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viridi-parente/refs/heads/main/openapi/viridi-parente-vista-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: viridiparente.com
  spf: true
hosts:
- cert_expires: Dec  1 08:44:47 2026 GMT
  host: viridiparente.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 02:01:36 2026 GMT
  host: vista.viridiparente.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Viridi Parente Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Viridi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Viridi
provider_slug: viridi-parente
slug: viridi-parente-domain-security
source_filename: viridi-parente-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: viridiparente.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 08:44:47 2026 GMT\n  hsts: false\n- host: vista.viridiparente.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 02:01:36 2026 GMT\n  hsts: false\ndomains:\n- domain: viridiparente.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viridi-parente/refs/heads/main/security/viridi-parente-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Energy Storage
- Battery
- IoT
- Industrial IoT
- Energy Management
- Manufacturing
- Telematics
- Microgrid
---
