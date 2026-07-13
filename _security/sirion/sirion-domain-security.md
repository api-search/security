---
api_specs:
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Contracts API
  slug: sirion-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Contract Requests API
  slug: sirion-contract-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Metadata & Clauses API
  slug: sirion-metadata-clauses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Obligations API
  slug: sirion-obligations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Suppliers & Counterparties API
  slug: sirion-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Integrations & Webhooks API
  slug: sirion-integrations-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sirion.ai
  spf: true
  spf_policy: -all
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sirioncloud.com
  spf: true
  spf_record: v=spf1 include:eu._netblocks.mimecast.com include:spf.protection.outlook.com include:sendgrid.net -all
hosts:
- cert_expires: Sep  9 05:30:25 2026 GMT
  cert_issuer: Let's Encrypt
  host: sirion.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Aug 18 05:41:43 2026 GMT
  cert_issuer: Let's Encrypt
  host: docs.sirion.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: Documentation portal on Document360 (CNAME lb-cdmz-kbv2.document360.io); login-walled.
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Aug 22 23:59:59 2026 GMT
  cert_issuer: DigiCert Inc
  host: app.sirioncloud.com
  hsts: false
  https: true
  note: Tenant application fronted by Akamai; bare host returns HTTP 400 (expects a tenant subdomain).
  server: AkamaiGHost
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sirion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sirion, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sirion
provider_slug: sirion
slug: sirion-domain-security
source_filename: sirion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of Sirion public hosts (2026-07-12)\nhosts:\n- host: sirion.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Sep  9 05:30:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  server: cloudflare\n- host: docs.sirion.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Aug 18 05:41:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  server: cloudflare\n  note: Documentation portal on Document360 (CNAME lb-cdmz-kbv2.document360.io); login-walled.\n- host: app.sirioncloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: DigiCert Inc\n  cert_expires: Aug 22 23:59:59 2026 GMT\n  hsts: false\n  server: AkamaiGHost\n  note: Tenant application fronted by Akamai; bare host returns HTTP 400 (expects a tenant subdomain).\ndomains:\n- domain: sirion.ai\n  dnssec: false\n\
  \  caa: []\n  spf: true\n  spf_policy: '-all'\n  dmarc: true\n  dmarc_policy: reject\n- domain: sirioncloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:eu._netblocks.mimecast.com include:spf.protection.outlook.com include:sendgrid.net -all\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/security/sirion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contract Management
- Contract Lifecycle Management
- CLM
- Contracts
- AI
- Enterprise
- Legal
- Agreements
- Supplier Management
- Obligations
---
