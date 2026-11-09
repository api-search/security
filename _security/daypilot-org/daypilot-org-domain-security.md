---
api_specs:
- filename: daypilot-org-discovery-api-openapi.yml
  format: yaml
  label: DayPilot Discovery API
  slug: daypilot-org-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daypilot-org/openapi/daypilot-org-discovery-api-openapi.yml
- filename: daypilot-org-generation-api-openapi.yml
  format: yaml
  label: DayPilot Generation API
  slug: daypilot-org-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daypilot-org/openapi/daypilot-org-generation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daypilot.org
  spf: true
hosts:
- cert_expires: Dec 12 14:51:24 2026 GMT
  host: daypilot.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Daypilot Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DayPilot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DayPilot
provider_slug: daypilot-org
slug: daypilot-org-domain-security
source_filename: daypilot-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daypilot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 14:51:24 2026 GMT\n  hsts: false\ndomains:\n- domain: daypilot.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/daypilot-org/security/daypilot-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Calendar
- Scheduler
- Gantt Chart
- UI Components
- Open Source
---
