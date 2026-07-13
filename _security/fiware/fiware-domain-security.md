---
api_specs:
- filename: fiware-ngsi-ld-openapi.yml
  format: yaml
  label: FIWARE NGSI-LD API
  slug: ngsi-ld
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-ngsi-ld-openapi.yml
- filename: fiware-ngsiv2-openapi.yml
  format: yaml
  label: FIWARE NGSI v2 API
  slug: ngsi-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-ngsiv2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fiware.org
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.fiware.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: orion.lab.fiware.org
  https: false
kind: domain-security
layout: security
method: probed
name: Fiware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FIWARE, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FIWARE
provider_slug: fiware
slug: fiware-domain-security
source_filename: fiware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fiware.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\n- host: orion.lab.fiware.org\n  https: false\ndomains:\n- domain: fiware.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/security/fiware-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Context Information
- Devices
- Internet of Things
- Linked Data
- NGSI
- Smart Cities
- Standards
---
