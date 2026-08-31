---
api_specs:
- filename: elemental-machines-alert-logs-api-openapi.yml
  format: yaml
  label: Elemental Machines Alert Logs API
  slug: elemental-machines-alert-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-alert-logs-api-openapi.yml
- filename: elemental-machines-alert-rules-api-openapi.yml
  format: yaml
  label: Elemental Machines Alert Rules API
  slug: elemental-machines-alert-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-alert-rules-api-openapi.yml
- filename: elemental-machines-authentication-api-openapi.yml
  format: yaml
  label: Elemental Machines Authentication API
  slug: elemental-machines-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-authentication-api-openapi.yml
- filename: elemental-machines-groups-api-openapi.yml
  format: yaml
  label: Elemental Machines Groups API
  slug: elemental-machines-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-groups-api-openapi.yml
- filename: elemental-machines-machines-api-openapi.yml
  format: yaml
  label: Elemental Machines Machines API
  slug: elemental-machines-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-machines-api-openapi.yml
- filename: elemental-machines-machines-sample-stats-api-openapi.yml
  format: yaml
  label: Elemental Machines Machines Sample Stats API
  slug: elemental-machines-machines-sample-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-machines-sample-stats-api-openapi.yml
- filename: elemental-machines-machines-samples-api-openapi.yml
  format: yaml
  label: Elemental Machines Machines Samples API
  slug: elemental-machines-machines-samples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-machines-samples-api-openapi.yml
- filename: elemental-machines-machines-usage-api-openapi.yml
  format: yaml
  label: Elemental Machines Machines Usage API
  slug: elemental-machines-machines-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-machines-usage-api-openapi.yml
- filename: elemental-machines-release-notes-api-openapi.yml
  format: yaml
  label: Elemental Machines Release Notes API
  slug: elemental-machines-release-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-release-notes-api-openapi.yml
- filename: elemental-machines-status-api-openapi.yml
  format: yaml
  label: Elemental Machines Status API
  slug: elemental-machines-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-status-api-openapi.yml
- filename: elemental-machines-user-activities-api-openapi.yml
  format: yaml
  label: Elemental Machines User Activities API
  slug: elemental-machines-user-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-user-activities-api-openapi.yml
- filename: elemental-machines-users-api-openapi.yml
  format: yaml
  label: Elemental Machines Users API
  slug: elemental-machines-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: elementalmachines.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: elementalmachines.io
  spf: true
hosts:
- cert_expires: Oct 26 22:27:21 2026 GMT
  host: elementalmachines.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 07:57:36 2026 GMT
  host: api.elementalmachines.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elemental Machines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elemental Machines, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Elemental Machines
provider_slug: elemental-machines
slug: elemental-machines-domain-security
source_filename: elemental-machines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elementalmachines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 22:27:21 2026 GMT\n  hsts: false\n- host: api.elementalmachines.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 07:57:36 2026 GMT\n  hsts: false\ndomains:\n- domain: elementalmachines.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: elementalmachines.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/security/elemental-machines-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- lab-operations
- laboratory-monitoring
- iot
- sensors
- life-sciences
- cold-chain
- environmental-monitoring
- equipment-utilization
- asset-management
- Alerting
- Compliance
- gxp
- Manufacturing
- time-series
---
