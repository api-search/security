---
api_specs:
- filename: zero-networks-ae-exclusions-api-openapi.yml
  format: yaml
  label: Zero Networks AE Exclusions API
  slug: zero-networks-ae-exclusions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-ae-exclusions-api-openapi.yml
- filename: zero-networks-assets-api-openapi.yml
  format: yaml
  label: Zero Networks Assets API
  slug: zero-networks-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-assets-api-openapi.yml
- filename: zero-networks-groups-custom-api-openapi.yml
  format: yaml
  label: Zero Networks Groups Custom API
  slug: zero-networks-groups-custom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-groups-custom-api-openapi.yml
- filename: zero-networks-internal-access-policy-api-openapi.yml
  format: yaml
  label: Zero Networks Internal Access Policy API
  slug: zero-networks-internal-access-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-internal-access-policy-api-openapi.yml
- filename: zero-networks-mfa-inbound-api-openapi.yml
  format: yaml
  label: Zero Networks MFA Inbound API
  slug: zero-networks-mfa-inbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-mfa-inbound-api-openapi.yml
- filename: zero-networks-mfa-outbound-api-openapi.yml
  format: yaml
  label: Zero Networks MFA Outbound API
  slug: zero-networks-mfa-outbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-mfa-outbound-api-openapi.yml
- filename: zero-networks-rules-inbound-api-openapi.yml
  format: yaml
  label: Zero Networks Rules Inbound API
  slug: zero-networks-rules-inbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-rules-inbound-api-openapi.yml
- filename: zero-networks-rules-outbound-api-openapi.yml
  format: yaml
  label: Zero Networks Rules Outbound API
  slug: zero-networks-rules-outbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-rules-outbound-api-openapi.yml
- filename: zero-networks-rules-rpc-api-openapi.yml
  format: yaml
  label: Zero Networks Rules RPC API
  slug: zero-networks-rules-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-rules-rpc-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zeronetworks.com
  spf: true
hosts:
- cert_expires: Oct  3 13:11:46 2026 GMT
  host: zeronetworks.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: portal.zeronetworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Zero Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zero Networks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zero Networks
provider_slug: zero-networks
slug: zero-networks-domain-security
source_filename: zero-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeronetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:11:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: portal.zeronetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zeronetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/security/zero-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Network Security
- Microsegmentation
- Zero Trust
- Identity
- Multi-Factor Authentication
- Segmentation
- ZTNA
- Kubernetes
- Cybersecurity
---
