---
api_specs:
- filename: pangea-ai-guard-api-openapi.yml
  format: yaml
  label: Pangea AI Guard API
  slug: pangea-ai-guard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-ai-guard-api-openapi.yml
- filename: pangea-authn-api-openapi.yml
  format: yaml
  label: Pangea AuthN API
  slug: pangea-authn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-authn-api-openapi.yml
- filename: pangea-domain-intel-api-openapi.yml
  format: yaml
  label: Pangea Domain Intel API
  slug: pangea-domain-intel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-domain-intel-api-openapi.yml
- filename: pangea-file-scan-api-openapi.yml
  format: yaml
  label: Pangea File Scan API
  slug: pangea-file-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-file-scan-api-openapi.yml
- filename: pangea-ip-intel-api-openapi.yml
  format: yaml
  label: Pangea IP Intel API
  slug: pangea-ip-intel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-ip-intel-api-openapi.yml
- filename: pangea-redact-api-openapi.yml
  format: yaml
  label: Pangea Redact API
  slug: pangea-redact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-redact-api-openapi.yml
- filename: pangea-secure-audit-log-api-openapi.yml
  format: yaml
  label: Pangea Secure Audit Log API
  slug: pangea-secure-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-secure-audit-log-api-openapi.yml
- filename: pangea-vault-api-openapi.yml
  format: yaml
  label: Pangea Vault API
  slug: pangea-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-vault-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pangea.cloud
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: pangea.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: authn.aws.us.pangea.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: audit.aws.us.pangea.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pangea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pangea, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pangea
provider_slug: pangea
slug: pangea-domain-security
source_filename: pangea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pangea.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: authn.aws.us.pangea.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\n- host: audit.aws.us.pangea.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: pangea.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/security/pangea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- AI Security
- Authentication
- Audit Log
- Data Protection
---
