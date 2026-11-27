---
api_specs:
- filename: clearhouse-sh-evidence-api-openapi.yml
  format: yaml
  label: Clearhouse Evidence API
  slug: clearhouse-sh-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearhouse-sh/openapi/clearhouse-sh-evidence-api-openapi.yml
- filename: clearhouse-sh-index-api-openapi.yml
  format: yaml
  label: Clearhouse Index API
  slug: clearhouse-sh-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearhouse-sh/openapi/clearhouse-sh-index-api-openapi.yml
- filename: clearhouse-sh-receipts-api-openapi.yml
  format: yaml
  label: Clearhouse Receipts API
  slug: clearhouse-sh-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearhouse-sh/openapi/clearhouse-sh-receipts-api-openapi.yml
- filename: clearhouse-sh-service-api-openapi.yml
  format: yaml
  label: Clearhouse Service API
  slug: clearhouse-sh-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearhouse-sh/openapi/clearhouse-sh-service-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clearhouse.sh
  spf: true
hosts:
- cert_expires: Jan 28 14:41:17 2027 GMT
  host: clearhouse.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clearhouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clearhouse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clearhouse
provider_slug: clearhouse-sh
slug: clearhouse-sh-domain-security
source_filename: clearhouse-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clearhouse.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 14:41:17 2027 GMT\n  hsts: false\ndomains:\n- domain: clearhouse.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/clearhouse-sh/security/clearhouse-sh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agent Registry
- Call Routing
- Signed Receipts
- Pay-per-call
- MCP
- A2A
---
