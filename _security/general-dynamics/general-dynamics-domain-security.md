---
api_specs:
- filename: general-dynamics-mission-systems-api-openapi.yml
  format: yaml
  label: General Dynamics Mission Systems API
  slug: mission-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/general-dynamics/refs/heads/main/openapi/general-dynamics-mission-systems-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gd.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gdmissionsystems.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.gd.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 22:16:25 2026 GMT
  host: gdmissionsystems.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.gdmissionsystems.com
  https: false
kind: domain-security
layout: security
method: probed
name: General Dynamics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for General Dynamics, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: General Dynamics
provider_slug: general-dynamics
slug: general-dynamics-domain-security
source_filename: general-dynamics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\n- host: gdmissionsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 22:16:25 2026 GMT\n  hsts: null\n- host: api.gdmissionsystems.com\n  https: false\ndomains:\n- domain: gd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gdmissionsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/general-dynamics/refs/heads/main/security/general-dynamics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aerospace
- Defense
- Mission Systems
- Government
- Fortune 100
---
