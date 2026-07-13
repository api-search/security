---
api_specs:
- filename: squadcast-openapi.yml
  format: yaml
  label: Squadcast Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squadcast/refs/heads/main/openapi/squadcast-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: squadcast.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: solarwinds.com
  spf: true
hosts:
- cert_expires: Sep 12 04:27:18 2026 GMT
  host: www.squadcast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 07:59:38 2026 GMT
  host: developers.incidents.cloud.solarwinds.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 09:00:29 2026 GMT
  host: api.squadcast.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Squadcast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Squadcast, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Squadcast
provider_slug: squadcast
slug: squadcast-domain-security
source_filename: squadcast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.squadcast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:27:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.incidents.cloud.solarwinds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 07:59:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.squadcast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 09:00:29 2026 GMT\n  hsts: null\ndomains:\n- domain: squadcast.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: solarwinds.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squadcast/refs/heads/main/security/squadcast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Incident Response
- On-Call Management
- DevOps
- SRE
- Alerting
- Incident Management
---
