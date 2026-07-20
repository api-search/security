---
api_specs:
- filename: esper-manage-openapi-original.yml
  format: yaml
  label: Esper Manage API
  slug: esper-manage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-manage-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: esper.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: esper.cloud
  spf: false
hosts:
- cert_expires: Oct 16 04:30:53 2026 GMT
  host: esper.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: api.esper.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: foo-api.esper.cloud
  https: false
kind: domain-security
layout: security
method: probed
name: Esper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Esper, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Esper
provider_slug: esper
slug: esper-domain-security
source_filename: esper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: esper.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 04:30:53 2026 GMT\n  hsts: false\n- host: api.esper.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: false\n- host: foo-api.esper.cloud\n  https: false\ndomains:\n- domain: esper.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: esper.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/security/esper-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Device Management
- Mobile Device Management
- Android
- DevOps
- Internet of Things
- Fleet Management
- Enterprise Mobility
- Edge Computing
- Kiosk
---
