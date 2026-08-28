---
api_specs:
- filename: nasuni-nmc-v1-2-openapi.yml
  format: yaml
  label: Nasuni Management Console (NMC) API
  slug: nasuni-management-console-nmc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasuni/refs/heads/main/openapi/nasuni-nmc-v1-2-openapi.yml
- filename: nasuni-portal-v0-openapi.yml
  format: yaml
  label: Nasuni Portal API
  slug: nasuni-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasuni/refs/heads/main/openapi/nasuni-portal-v0-openapi.yml
- filename: nasuni-global-file-acceleration-telemetry-openapi.yml
  format: yaml
  label: Global File Acceleration (GFA) Telemetry API
  slug: global-file-acceleration-gfa-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasuni/refs/heads/main/openapi/nasuni-global-file-acceleration-telemetry-openapi.yml
- filename: nasuni-nasuni-data-service-azure-openapi.yml
  format: yaml
  label: Nasuni Data Service (NDS) for Azure API
  slug: nasuni-data-service-nds-for-azure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasuni/refs/heads/main/openapi/nasuni-nasuni-data-service-azure-openapi.yml
- filename: nasuni-nasuni-data-service-aws-openapi.yml
  format: yaml
  label: Nasuni Data Service (NDS) for AWS API
  slug: nasuni-data-service-nds-for-aws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasuni/refs/heads/main/openapi/nasuni-nasuni-data-service-aws-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nasuni.com
  spf: true
hosts:
- cert_expires: Oct  4 19:33:03 2026 GMT
  host: www.nasuni.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 16:59:36 2026 GMT
  host: docs.api.nasuni.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: am1.portal.api.nasuni.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nasuni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nasuni, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nasuni
provider_slug: nasuni
slug: nasuni-domain-security
source_filename: nasuni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nasuni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:33:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.api.nasuni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:59:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: am1.portal.api.nasuni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nasuni.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasuni/refs/heads/main/security/nasuni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- File Storage
- Hybrid Cloud
- Object Storage
- Enterprise Storage
- Data Management
- Backup and Recovery
- Ransomware Protection
- Infrastructure
- Observability
- MCP
- agent-native
---
