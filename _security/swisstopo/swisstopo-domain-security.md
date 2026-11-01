---
api_specs:
- filename: swisstopo-layers-api-openapi.yml
  format: yaml
  label: swisstopo Layers API
  slug: swisstopo-layers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swisstopo/openapi/swisstopo-layers-api-openapi.yml
- filename: swisstopo-vocabularies-api-openapi.yml
  format: yaml
  label: swisstopo Vocabularies API
  slug: swisstopo-vocabularies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swisstopo/openapi/swisstopo-vocabularies-api-openapi.yml
- filename: swisstopo-wms-api-openapi.yml
  format: yaml
  label: swisstopo WMS API
  slug: swisstopo-wms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swisstopo/openapi/swisstopo-wms-api-openapi.yml
- filename: swisstopo-wmts-api-openapi.yml
  format: yaml
  label: swisstopo WMTS API
  slug: swisstopo-wmts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swisstopo/openapi/swisstopo-wmts-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "certainly.com"
  - 0 iodef "mailto:hostmaster@admin.ch"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "swisssign.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: admin.ch
  spf: true
hosts:
- cert_expires: Nov 27 13:22:48 2026 GMT
  host: www.swisstopo.admin.ch
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Swisstopo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for swisstopo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: swisstopo
provider_slug: swisstopo
slug: swisstopo-domain-security
source_filename: swisstopo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swisstopo.admin.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 13:22:48 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: admin.ch\n  dnssec: false\n  caa:\n  - 0 issue \"certainly.com\"\n  - 0 iodef \"mailto:hostmaster@admin.ch\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"swisssign.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/swisstopo/security/swisstopo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geodata
- Government
- Switzerland
- Mapping
- OpenData
---
