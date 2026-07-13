---
api_specs:
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea AuthN API
  slug: authn
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea Secure Audit Log API
  slug: secure-audit-log
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea Redact API
  slug: redact
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea Vault API
  slug: vault
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea File Scan API
  slug: file-scan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea IP Intel API
  slug: ip-intel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea Domain & URL Intel API
  slug: domain-intel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea AI Guard & Prompt Guard API
  slug: ai-guard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
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
