---
api_specs:
- filename: api-reference
  format: yaml
  label: Basware P2P API
  slug: basware-p2p-api
  spec_type: OpenAPI
  url: https://developer.basware.com/en/api/basware/api-reference
- filename: api-reference
  format: yaml
  label: Basware Network API
  slug: basware-network-api
  spec_type: OpenAPI
  url: https://developer.basware.com/en/api/network/api-reference
- filename: basware-vault-openapi.yaml
  format: yaml
  label: Basware Vault API
  slug: basware-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basware/refs/heads/main/openapi/basware-vault-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: basware.com
  spf: true
hosts:
- cert_expires: Oct  4 09:55:29 2026 GMT
  host: www.basware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 16:21:09 2026 GMT
  host: developer.basware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 10 07:08:25 2027 GMT
  host: api.basware.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Basware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basware, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Basware
provider_slug: basware
slug: basware-domain-security
source_filename: basware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.basware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 09:55:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.basware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:21:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.basware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 07:08:25 2027 GMT\n  hsts: null\ndomains:\n- domain: basware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basware/refs/heads/main/security/basware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Invoicing
- Purchase-to-Pay
- Accounts Payable
- Procurement
- Electronic Invoicing
- Finance Automation
- B2B Payments
---
