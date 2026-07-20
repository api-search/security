---
api_specs:
- filename: b3-b3os-workflow-openapi.json
  format: json
  label: B3OS Workflow API
  slug: b3os-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3/refs/heads/main/openapi/b3-b3os-workflow-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: b3.fun
  spf: true
hosts:
- cert_expires: Sep  3 07:15:07 2026 GMT
  host: b3.fun
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: B3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for B3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: B3
provider_slug: b3
slug: b3-domain-security
source_filename: b3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: b3.fun\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 07:15:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: b3.fun\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b3/refs/heads/main/security/b3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Blockchain
- Web3
- Workflow Automation
- Onchain Data
- Gaming
- Payments
- Layer 3
- Developer Tools
---
