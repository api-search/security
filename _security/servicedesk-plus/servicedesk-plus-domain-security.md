---
api_specs:
- filename: servicedesk-plus-openapi.yml
  format: yaml
  label: ServiceDesk Plus REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicedesk-plus/refs/heads/main/openapi/servicedesk-plus-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: manageengine.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: manageengine.eu
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: www.manageengine.com
  hsts: true
  hsts_max_age: 64072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: sdpondemand.manageengine.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: sdpondemand.manageengine.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Servicedesk Plus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ManageEngine ServiceDesk Plus, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ManageEngine ServiceDesk Plus
provider_slug: servicedesk-plus
slug: servicedesk-plus-domain-security
source_filename: servicedesk-plus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.manageengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 64072000\n- host: sdpondemand.manageengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\n- host: sdpondemand.manageengine.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: manageengine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: manageengine.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicedesk-plus/refs/heads/main/security/servicedesk-plus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ITSM
- Help Desk
- Incident Management
- Asset Management
- CMDB
---
