---
api_specs:
- filename: printnode-openapi.yml
  format: yaml
  label: PrintNode Computers API
  slug: computers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-openapi.yml
- filename: printnode-openapi.yml
  format: yaml
  label: PrintNode Printers API
  slug: printers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-openapi.yml
- filename: printnode-openapi.yml
  format: yaml
  label: PrintNode PrintJobs API
  slug: printjobs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-openapi.yml
- filename: printnode-openapi.yml
  format: yaml
  label: PrintNode Scales API
  slug: scales
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-openapi.yml
- filename: printnode-openapi.yml
  format: yaml
  label: PrintNode Account and API Keys API
  slug: account-api-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-openapi.yml
- filename: printnode-openapi.yml
  format: yaml
  label: PrintNode Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: printnode.com
  spf: true
hosts:
- cert_expires: Oct 16 14:16:31 2026 GMT
  host: www.printnode.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 14:16:31 2026 GMT
  host: api.printnode.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Printnode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PrintNode, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PrintNode
provider_slug: printnode
slug: printnode-domain-security
source_filename: printnode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.printnode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:16:31 2026 GMT\n  hsts: null\n- host: api.printnode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:16:31 2026 GMT\n  hsts: null\ndomains:\n- domain: printnode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/security/printnode-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Printing
- Cloud Printing
- Remote Printing
- Print Jobs
- Hardware
---
