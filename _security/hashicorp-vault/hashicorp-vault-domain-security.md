---
api_specs:
- filename: hashicorp-vault-auth-approle-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Auth - AppRole API
  slug: hashicorp-vault-auth-approle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-auth-approle-api-openapi.yml
- filename: hashicorp-vault-auth-token-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Auth - Token API
  slug: hashicorp-vault-auth-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-auth-token-api-openapi.yml
- filename: hashicorp-vault-auth-userpass-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Auth - Userpass API
  slug: hashicorp-vault-auth-userpass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-auth-userpass-api-openapi.yml
- filename: hashicorp-vault-identity-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Identity API
  slug: hashicorp-vault-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-identity-api-openapi.yml
- filename: hashicorp-vault-leases-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Leases API
  slug: hashicorp-vault-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-leases-api-openapi.yml
- filename: hashicorp-vault-policy-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Policy API
  slug: hashicorp-vault-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-policy-api-openapi.yml
- filename: hashicorp-vault-secrets-kv-v2-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Secrets - KV v2 API
  slug: hashicorp-vault-secrets-kv-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-secrets-kv-v2-api-openapi.yml
- filename: hashicorp-vault-secrets-transit-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Secrets - Transit API
  slug: hashicorp-vault-secrets-transit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-secrets-transit-api-openapi.yml
- filename: hashicorp-vault-system-api-openapi.yml
  format: yaml
  label: HashiCorp Vault System API
  slug: hashicorp-vault-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vaultproject.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hashicorp.com
  spf: true
hosts:
- cert_expires: Sep  3 10:34:37 2026 GMT
  host: www.vaultproject.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 05:45:45 2026 GMT
  host: developer.hashicorp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Hashicorp Vault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HashiCorp Vault, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HashiCorp Vault
provider_slug: hashicorp-vault
slug: hashicorp-vault-domain-security
source_filename: hashicorp-vault-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vaultproject.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 10:34:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.hashicorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: vaultproject.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hashicorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/security/hashicorp-vault-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DevOps
- Encryption
- Infrastructure
- Secrets Management
- Security
---
