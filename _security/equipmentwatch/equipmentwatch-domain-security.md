---
api_specs:
- filename: equipmentwatch-api-openapi.yaml
  format: yaml
  label: EquipmentWatch Taxonomy API
  slug: taxonomy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-api-openapi.yaml
- filename: equipmentwatch-api-openapi.yaml
  format: yaml
  label: EquipmentWatch Specs API
  slug: specs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-api-openapi.yaml
- filename: equipmentwatch-api-openapi.yaml
  format: yaml
  label: EquipmentWatch Verification API
  slug: verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-api-openapi.yaml
- filename: equipmentwatch-api-openapi.yaml
  format: yaml
  label: EquipmentWatch Costs API
  slug: costs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-api-openapi.yaml
- filename: equipmentwatch-api-openapi.yaml
  format: yaml
  label: EquipmentWatch Values API
  slug: values
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-api-openapi.yaml
- filename: equipmentwatch-api-openapi.yaml
  format: yaml
  label: EquipmentWatch Retail Rental API
  slug: retail-rental
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: equipmentwatch.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: equipmentwatchapi.com
  spf: false
hosts:
- cert_expires: Nov 12 14:27:14 2026 GMT
  host: www.equipmentwatch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 22:28:54 2026 GMT
  host: equipmentwatch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: equipmentwatchapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Equipmentwatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equipmentwatch, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Equipmentwatch
provider_slug: equipmentwatch
slug: equipmentwatch-domain-security
source_filename: equipmentwatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.equipmentwatch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 14:27:14 2026 GMT\n  hsts: false\n- host: equipmentwatch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 22:28:54 2026 GMT\n  hsts: false\n- host: equipmentwatchapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: equipmentwatch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: equipmentwatchapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/security/equipmentwatch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Construction
- Equipment
- Rental Rates
- Valuation
- Heavy Equipment
- Equipment Data
- Market Data
---
