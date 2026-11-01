---
api_specs:
- filename: divineapi-com-openapi.yml
  format: yaml
  label: DivineAPI
  slug: divineapi
  spec_type: OpenAPI
  url: https://artifacts.apis.io/divineapi-com/openapi/divineapi-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: divineapi.com
  spf: true
hosts:
- cert_expires: Jan 24 08:48:36 2027 GMT
  host: divineapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Divineapi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for divineapi-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: divineapi-com
provider_slug: divineapi-com
slug: divineapi-com-domain-security
source_filename: divineapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: divineapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 08:48:36 2027 GMT\n  hsts: false\ndomains:\n- domain: divineapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/divineapi-com/security/divineapi-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Astrology
- API
- Data
- Developer
- Platform
---
