---
api_specs:
- filename: elemental-machines-api-openapi.yml
  format: yaml
  label: Elemental Machines API
  slug: elemental-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: elementalmachines.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: elementalmachines.io
  spf: true
hosts:
- cert_expires: Oct 26 22:27:21 2026 GMT
  host: elementalmachines.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 07:57:36 2026 GMT
  host: api.elementalmachines.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elemental Machines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elemental Machines, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Elemental Machines
provider_slug: elemental-machines
slug: elemental-machines-domain-security
source_filename: elemental-machines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elementalmachines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 22:27:21 2026 GMT\n  hsts: false\n- host: api.elementalmachines.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 07:57:36 2026 GMT\n  hsts: false\ndomains:\n- domain: elementalmachines.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: elementalmachines.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/security/elemental-machines-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- lab-operations
- laboratory-monitoring
- iot
- sensors
- life-sciences
- cold-chain
- environmental-monitoring
- equipment-utilization
- asset-management
- alerting
- compliance
- gxp
- manufacturing
- time-series
---
