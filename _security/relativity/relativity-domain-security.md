---
api_specs:
- filename: relativity-object-manager-openapi.yml
  format: yaml
  label: Relativity Object Manager API
  slug: relativity-object-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-object-manager-openapi.yml
- filename: relativity-import-openapi.yml
  format: yaml
  label: Relativity Import Service API
  slug: relativity-import-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-import-openapi.yml
- filename: relativity-export-openapi.yml
  format: yaml
  label: Relativity Export Service API
  slug: relativity-export-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-export-openapi.yml
- filename: relativity-workspace-openapi.yml
  format: yaml
  label: Relativity Workspace Manager API
  slug: relativity-workspace-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-workspace-openapi.yml
- filename: relativity-productions-openapi.yml
  format: yaml
  label: Relativity Production Manager API
  slug: relativity-production-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-productions-openapi.yml
- filename: relativity-legal-hold-openapi.yml
  format: yaml
  label: Relativity Legal Hold API
  slug: relativity-legal-hold-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-legal-hold-openapi.yml
- filename: relativity-automated-workflows-openapi.yml
  format: yaml
  label: Relativity Automated Workflows API
  slug: relativity-automated-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-automated-workflows-openapi.yml
- filename: relativity-permissions-openapi.yml
  format: yaml
  label: Relativity Audit API
  slug: relativity-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-permissions-openapi.yml
- filename: relativity-identity-openapi.yml
  format: yaml
  label: Relativity User and Permission Manager API
  slug: relativity-user-and-permission-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-identity-openapi.yml
- filename: relativity-billing-v2-openapi.yml
  format: yaml
  label: Relativity Billing Insights API
  slug: relativity-billing-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-billing-v2-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "intermediatecertificate.digitalcertvalidation.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "rapidssl.com"
  - 0 issuewild "stratossl.digitalcertvalidation.com"
  - 0 issuewild "thawte.com"
  - 0 issuewild "volusion.digitalcertvalidation.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: relativity.com
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: platform.relativity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: help.relativity.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Relativity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relativity, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Relativity
provider_slug: relativity
slug: relativity-domain-security
source_filename: relativity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platform.relativity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.relativity.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: relativity.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"intermediatecertificate.digitalcertvalidation.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"rapidssl.com\"\n  - 0 issuewild \"stratossl.digitalcertvalidation.com\"\n  - 0 issuewild \"thawte.com\"\n  - 0 issuewild \"volusion.digitalcertvalidation.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/security/relativity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eDiscovery
- Legal
- Document Review
- Legal Technology
- Data Processing
- AI Review
- Litigation
- Compliance
---
