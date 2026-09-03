---
api_specs:
- filename: agco-locations-api-openapi.yml
  format: yaml
  label: agco Locations API
  slug: agco-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/openapi/agco-locations-api-openapi.yml
- filename: agco-machines-api-openapi.yml
  format: yaml
  label: agco Machines API
  slug: agco-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/openapi/agco-machines-api-openapi.yml
- filename: agco-telemetry-api-openapi.yml
  format: yaml
  label: agco Telemetry API
  slug: agco-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/openapi/agco-telemetry-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agcoconnect.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agcocorp.com
  spf: true
hosts:
- cert_expires: Sep  9 03:08:26 2026 GMT
  host: get.agcoconnect.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: api.agcocorp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agco, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agco
provider_slug: agco
slug: agco-domain-security
source_filename: agco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: get.agcoconnect.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  9 03:08:26 2026 GMT\n  hsts: false\n- host: api.agcocorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: agcoconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: agcocorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/security/agco-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Fortune 500
---
