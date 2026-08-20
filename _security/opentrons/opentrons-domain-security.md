---
api_specs:
- filename: opentrons-attached-instruments-api-openapi.yml
  format: yaml
  label: Opentrons Attached Instruments API
  slug: opentrons-attached-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentrons/refs/heads/main/openapi/opentrons-attached-instruments-api-openapi.yml
- filename: opentrons-attached-modules-api-openapi.yml
  format: yaml
  label: Opentrons Attached Modules API
  slug: opentrons-attached-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentrons/refs/heads/main/openapi/opentrons-attached-modules-api-openapi.yml
- filename: opentrons-flex-deck-configuration-api-openapi.yml
  format: yaml
  label: Opentrons Flex Deck Configuration API
  slug: opentrons-flex-deck-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentrons/refs/heads/main/openapi/opentrons-flex-deck-configuration-api-openapi.yml
- filename: opentrons-health-api-openapi.yml
  format: yaml
  label: Opentrons Health API
  slug: opentrons-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentrons/refs/heads/main/openapi/opentrons-health-api-openapi.yml
- filename: opentrons-protocol-management-api-openapi.yml
  format: yaml
  label: Opentrons Protocol Management API
  slug: opentrons-protocol-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentrons/refs/heads/main/openapi/opentrons-protocol-management-api-openapi.yml
- filename: opentrons-robot-api-openapi.yml
  format: yaml
  label: Opentrons Robot API
  slug: opentrons-robot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentrons/refs/heads/main/openapi/opentrons-robot-api-openapi.yml
- filename: opentrons-run-management-api-openapi.yml
  format: yaml
  label: Opentrons Run Management API
  slug: opentrons-run-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentrons/refs/heads/main/openapi/opentrons-run-management-api-openapi.yml
- filename: opentrons-simple-commands-api-openapi.yml
  format: yaml
  label: Opentrons Simple Commands API
  slug: opentrons-simple-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentrons/refs/heads/main/openapi/opentrons-simple-commands-api-openapi.yml
- filename: opentrons-system-control-api-openapi.yml
  format: yaml
  label: Opentrons System Control API
  slug: opentrons-system-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentrons/refs/heads/main/openapi/opentrons-system-control-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opentrons.com
  spf: true
hosts:
- cert_expires: Oct  5 00:04:46 2026 GMT
  host: opentrons.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: docs.opentrons.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opentrons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opentrons, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Opentrons
provider_slug: opentrons
slug: opentrons-domain-security
source_filename: opentrons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opentrons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:04:46 2026 GMT\n  hsts: false\n- host: docs.opentrons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: opentrons.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opentrons/refs/heads/main/security/opentrons-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Lab Automation
- Liquid Handling
- Robotics
- Biology
- Life Sciences
- Protocol Management
- Hardware Control
- Open-Source
---
