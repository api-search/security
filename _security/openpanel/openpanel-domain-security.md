---
api_specs:
- filename: openpanel-openapi.yml
  format: yaml
  label: OpenPanel API
  slug: openpanel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpanel/refs/heads/main/openapi/openpanel-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openpanel.dev
  spf: true
hosts:
- cert_expires: Sep 29 23:30:29 2026 GMT
  host: openpanel.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 09:31:45 2026 GMT
  host: api.openpanel.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openpanel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenPanel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OpenPanel
provider_slug: openpanel
slug: openpanel-domain-security
source_filename: openpanel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openpanel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:30:29 2026 GMT\n  hsts: false\n- host: api.openpanel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 09:31:45 2026 GMT\n  hsts: false\ndomains:\n- domain: openpanel.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpanel/refs/heads/main/security/openpanel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Event Tracking
- Funnels
- Open Source
- Product Analytics
- Real-Time Analytics
- User Analytics
---
