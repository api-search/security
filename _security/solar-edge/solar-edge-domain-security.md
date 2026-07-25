---
api_specs:
- filename: solar-edge-accounts-api-openapi.yml
  format: yaml
  label: SolarEdge Accounts API
  slug: solar-edge-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-accounts-api-openapi.yml
- filename: solar-edge-energy-api-openapi.yml
  format: yaml
  label: SolarEdge Energy API
  slug: solar-edge-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-energy-api-openapi.yml
- filename: solar-edge-environmental-api-openapi.yml
  format: yaml
  label: SolarEdge Environmental API
  slug: solar-edge-environmental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-environmental-api-openapi.yml
- filename: solar-edge-equipment-api-openapi.yml
  format: yaml
  label: SolarEdge Equipment API
  slug: solar-edge-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-equipment-api-openapi.yml
- filename: solar-edge-power-api-openapi.yml
  format: yaml
  label: SolarEdge Power API
  slug: solar-edge-power-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-power-api-openapi.yml
- filename: solar-edge-sites-api-openapi.yml
  format: yaml
  label: SolarEdge Sites API
  slug: solar-edge-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-sites-api-openapi.yml
- filename: solar-edge-storage-api-openapi.yml
  format: yaml
  label: SolarEdge Storage API
  slug: solar-edge-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-storage-api-openapi.yml
- filename: solar-edge-version-api-openapi.yml
  format: yaml
  label: SolarEdge Version API
  slug: solar-edge-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-version-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: solaredge.com
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.solaredge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: developers.solaredge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: monitoringapi.solaredge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solar Edge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SolarEdge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SolarEdge
provider_slug: solar-edge
slug: solar-edge-domain-security
source_filename: solar-edge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solaredge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\n- host: developers.solaredge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\n- host: monitoringapi.solaredge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: solaredge.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/security/solar-edge-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Solar
- Energy
- Monitoring
- PV
- Inverter
- Renewable Energy
- IoT
---
