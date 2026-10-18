---
api_specs:
- filename: machinemetrics-machinemetrics-api-api-openapi.yml
  format: yaml
  label: MachineMetrics MachineMetrics API
  slug: machinemetrics-machinemetrics-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinemetrics/refs/heads/main/openapi/machinemetrics-machinemetrics-api-api-openapi.yml
- filename: machinemetrics-mmdevcli-api-openapi.yml
  format: yaml
  label: MachineMetrics Mmdevcli API
  slug: machinemetrics-mmdevcli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinemetrics/refs/heads/main/openapi/machinemetrics-mmdevcli-api-openapi.yml
- filename: machinemetrics-ping-api-openapi.yml
  format: yaml
  label: MachineMetrics Ping API
  slug: machinemetrics-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinemetrics/refs/heads/main/openapi/machinemetrics-ping-api-openapi.yml
- filename: machinemetrics-reports-api-openapi.yml
  format: yaml
  label: MachineMetrics Reports API
  slug: machinemetrics-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinemetrics/refs/heads/main/openapi/machinemetrics-reports-api-openapi.yml
- filename: machinemetrics-graph-ql-api-openapi.yml
  format: yaml
  label: MachineMetrics Graph QL API
  slug: machinemetrics-graph-ql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinemetrics/refs/heads/main/openapi/machinemetrics-graph-ql-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: machinemetrics.com
  spf: true
hosts:
- cert_expires: Nov 17 22:01:49 2026 GMT
  host: www.machinemetrics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Machinemetrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MachineMetrics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MachineMetrics
provider_slug: machinemetrics
slug: machinemetrics-domain-security
source_filename: machinemetrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.machinemetrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 22:01:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: machinemetrics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machinemetrics/refs/heads/main/security/machinemetrics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- Artificial Intelligence
- MES
- IoT
- Software-as-a-Service
---
