---
api_specs:
- filename: wayflyer-auth-api-openapi.yml
  format: yaml
  label: Wayflyer Auth API
  slug: wayflyer-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-auth-api-openapi.yml
- filename: wayflyer-company-details-api-openapi.yml
  format: yaml
  label: Wayflyer Company Details API
  slug: wayflyer-company-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-company-details-api-openapi.yml
- filename: wayflyer-company-search-api-openapi.yml
  format: yaml
  label: Wayflyer Company Search API
  slug: wayflyer-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-company-search-api-openapi.yml
- filename: wayflyer-cta-api-openapi.yml
  format: yaml
  label: Wayflyer CTA API
  slug: wayflyer-cta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-cta-api-openapi.yml
- filename: wayflyer-data-upload-api-openapi.yml
  format: yaml
  label: Wayflyer Data Upload API
  slug: wayflyer-data-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-data-upload-api-openapi.yml
- filename: wayflyer-documents-api-openapi.yml
  format: yaml
  label: Wayflyer Documents API
  slug: wayflyer-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-documents-api-openapi.yml
- filename: wayflyer-embedded-application-api-openapi.yml
  format: yaml
  label: Wayflyer Embedded Application API
  slug: wayflyer-embedded-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-embedded-application-api-openapi.yml
- filename: wayflyer-handover-api-openapi.yml
  format: yaml
  label: Wayflyer Handover API
  slug: wayflyer-handover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-handover-api-openapi.yml
- filename: wayflyer-industry-classification-api-openapi.yml
  format: yaml
  label: Wayflyer Industry Classification API
  slug: wayflyer-industry-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-industry-classification-api-openapi.yml
- filename: wayflyer-simulation-api-openapi.yml
  format: yaml
  label: Wayflyer Simulation API
  slug: wayflyer-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-simulation-api-openapi.yml
- filename: wayflyer-tracked-login-api-openapi.yml
  format: yaml
  label: Wayflyer Tracked Login API
  slug: wayflyer-tracked-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-tracked-login-api-openapi.yml
- filename: wayflyer-user-details-api-openapi.yml
  format: yaml
  label: Wayflyer User Details API
  slug: wayflyer-user-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-user-details-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wayflyer.com
  spf: true
hosts:
- cert_expires: Sep 13 10:36:38 2026 GMT
  host: wayflyer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.wayflyer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: sandbox-api.wayflyer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wayflyer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wayflyer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wayflyer
provider_slug: wayflyer
slug: wayflyer-domain-security
source_filename: wayflyer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wayflyer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 10:36:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.wayflyer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: false\n- host: sandbox-api.wayflyer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: wayflyer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/security/wayflyer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Fintech
- Embedded Finance
- Lending
- Revenue-Based Financing
- Financing
---
