---
api_specs:
- filename: phala-apps-api-openapi.yml
  format: yaml
  label: Phala Network Apps API
  slug: phala-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-apps-api-openapi.yml
- filename: phala-apps-kms-info-api-openapi.yml
  format: yaml
  label: Phala Network Apps Kms Info API
  slug: phala-apps-kms-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-apps-kms-info-api-openapi.yml
- filename: phala-apps-pending-updates-api-openapi.yml
  format: yaml
  label: Phala Network Apps Pending Updates API
  slug: phala-apps-pending-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-apps-pending-updates-api-openapi.yml
- filename: phala-attestations-api-openapi.yml
  format: yaml
  label: Phala Network Attestations API
  slug: phala-attestations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-attestations-api-openapi.yml
- filename: phala-cvms-api-openapi.yml
  format: yaml
  label: Phala Network CVMs API
  slug: phala-cvms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-cvms-api-openapi.yml
- filename: phala-cvms-network-config-api-openapi.yml
  format: yaml
  label: Phala Network Cvms Network Config API
  slug: phala-cvms-network-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-cvms-network-config-api-openapi.yml
- filename: phala-instance-types-api-openapi.yml
  format: yaml
  label: Phala Network Instance Types API
  slug: phala-instance-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-instance-types-api-openapi.yml
- filename: phala-kms-api-openapi.yml
  format: yaml
  label: Phala Network KMS API
  slug: phala-kms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-kms-api-openapi.yml
- filename: phala-ssh-keys-api-openapi.yml
  format: yaml
  label: Phala Network SSH Keys API
  slug: phala-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-ssh-keys-api-openapi.yml
- filename: phala-webhooks-api-openapi.yml
  format: yaml
  label: Phala Network Webhooks API
  slug: phala-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: phala.network
  spf: true
hosts:
- cert_expires: Dec  3 22:30:31 2026 GMT
  host: phala.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Phala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phala Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Phala Network
provider_slug: phala
slug: phala-domain-security
source_filename: phala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phala.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 22:30:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: phala.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/security/phala-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Confidential Computing
- Trusted Execution Environments
- Inference
- Cloud Infrastructure
- Attestation
- LLM Router
---
