---
api_specs:
- filename: hvault-system-backend-openapi.yml
  format: yaml
  label: Vault System Backend API
  slug: vault-system-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/openapi/hvault-system-backend-openapi.yml
- filename: hvault-secrets-engines-openapi.yml
  format: yaml
  label: Vault Secrets Engines API
  slug: vault-secrets-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/openapi/hvault-secrets-engines-openapi.yml
- filename: hvault-auth-methods-openapi.yml
  format: yaml
  label: Vault Auth Methods API
  slug: vault-auth-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/openapi/hvault-auth-methods-openapi.yml
- filename: hvault-identity-openapi.yml
  format: yaml
  label: Vault Identity API
  slug: vault-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/openapi/hvault-identity-openapi.yml
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
kind: domain-security
layout: security
method: probed
name: Hvault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HashiCorp Vault, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HashiCorp Vault
provider_slug: hvault
slug: hvault-domain-security
source_filename: hvault-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vaultproject.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 10:34:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.hashicorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vaultproject.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hashicorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/security/hvault-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Encryption
- Identity
- Infrastructure
- Secrets Management
- Security
---
