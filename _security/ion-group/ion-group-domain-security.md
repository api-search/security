---
api_specs:
- filename: ion-group-openapi.yml
  format: yaml
  label: Ion Group Acuris Entities API
  slug: acuris-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ion-group/refs/heads/main/openapi/ion-group-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iongroup.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acuris.com
  spf: true
hosts:
- cert_expires: Sep 13 12:41:49 2026 GMT
  host: iongroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 14 01:25:15 2027 GMT
  host: api.acuris.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ion Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ion Group, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ion Group
provider_slug: ion-group
slug: ion-group-domain-security
source_filename: ion-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iongroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 12:41:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.acuris.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 14 01:25:15 2027 GMT\n  hsts: false\ndomains:\n- domain: iongroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: acuris.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ion-group/refs/heads/main/security/ion-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Financial
- Financial Services
- Trading
---
