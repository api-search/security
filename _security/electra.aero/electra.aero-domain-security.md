---
api_specs:
- filename: electra.aero-content-openapi.yml
  format: yaml
  label: Electra.aero Content API
  slug: electraaero-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electra.aero/refs/heads/main/openapi/electra.aero-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: electra.aero
  spf: true
hosts:
- cert_expires: Oct 25 02:12:00 2026 GMT
  host: electra.aero
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Electra.Aero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Electra.aero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Electra.aero
provider_slug: electra.aero
slug: electra.aero-domain-security
source_filename: electra.aero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: electra.aero\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 02:12:00 2026 GMT\n  hsts: false\ndomains:\n- domain: electra.aero\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electra.aero/refs/heads/main/security/electra.aero-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aerospace
- Aviation
- Aircraft Manufacturing
- Advanced Air Mobility
- Electric Aviation
- Hybrid-Electric Propulsion
- Regional Air Mobility
- Defense
- Transportation
- Content
- Company
---
