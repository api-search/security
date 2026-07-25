---
api_specs:
- filename: port-community-systems-cargomanifests-api-openapi.yml
  format: yaml
  label: Port Community Systems CargoManifests API
  slug: port-community-systems-cargomanifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/openapi/port-community-systems-cargomanifests-api-openapi.yml
- filename: port-community-systems-containers-api-openapi.yml
  format: yaml
  label: Port Community Systems Containers API
  slug: port-community-systems-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/openapi/port-community-systems-containers-api-openapi.yml
- filename: port-community-systems-customsdeclarations-api-openapi.yml
  format: yaml
  label: Port Community Systems CustomsDeclarations API
  slug: port-community-systems-customsdeclarations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/openapi/port-community-systems-customsdeclarations-api-openapi.yml
- filename: port-community-systems-hazardouscargo-api-openapi.yml
  format: yaml
  label: Port Community Systems HazardousCargo API
  slug: port-community-systems-hazardouscargo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/openapi/port-community-systems-hazardouscargo-api-openapi.yml
- filename: port-community-systems-vesselcalls-api-openapi.yml
  format: yaml
  label: Port Community Systems VesselCalls API
  slug: port-community-systems-vesselcalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/openapi/port-community-systems-vesselcalls-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ipcsa.international
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: portbase.com
  spf: true
hosts:
- cert_expires: Oct  3 20:02:47 2026 GMT
  host: www.ipcsa.international
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: www.portbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 07:02:10 2026 GMT
  host: api.portbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Port Community Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Port Community Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Port Community Systems
provider_slug: port-community-systems
slug: port-community-systems-domain-security
source_filename: port-community-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ipcsa.international\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:02:47 2026 GMT\n  hsts: false\n- host: www.portbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.portbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 07:02:10 2026 GMT\n  hsts: null\ndomains:\n- domain: ipcsa.international\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: portbase.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/security/port-community-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Maritime
- Port
- Logistics
- Customs
- Cargo
- Shipping
---
