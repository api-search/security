---
api_specs:
- filename: printnode-account-api-openapi.yml
  format: yaml
  label: PrintNode Account API
  slug: printnode-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-account-api-openapi.yml
- filename: printnode-api-keys-api-openapi.yml
  format: yaml
  label: PrintNode API Keys API
  slug: printnode-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-api-keys-api-openapi.yml
- filename: printnode-clients-api-openapi.yml
  format: yaml
  label: PrintNode Clients API
  slug: printnode-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-clients-api-openapi.yml
- filename: printnode-computers-api-openapi.yml
  format: yaml
  label: PrintNode Computers API
  slug: printnode-computers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-computers-api-openapi.yml
- filename: printnode-printers-api-openapi.yml
  format: yaml
  label: PrintNode Printers API
  slug: printnode-printers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-printers-api-openapi.yml
- filename: printnode-printjobs-api-openapi.yml
  format: yaml
  label: PrintNode PrintJobs API
  slug: printnode-printjobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-printjobs-api-openapi.yml
- filename: printnode-scales-api-openapi.yml
  format: yaml
  label: PrintNode Scales API
  slug: printnode-scales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-scales-api-openapi.yml
- filename: printnode-utility-api-openapi.yml
  format: yaml
  label: PrintNode Utility API
  slug: printnode-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-utility-api-openapi.yml
- filename: printnode-webhooks-api-openapi.yml
  format: yaml
  label: PrintNode Webhooks API
  slug: printnode-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-webhooks-api-openapi.yml
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
