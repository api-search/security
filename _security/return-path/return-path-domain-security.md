---
api_specs:
- filename: return-path-account-services-api-openapi.yml
  format: yaml
  label: Return Path Account Services API
  slug: return-path-account-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-account-services-api-openapi.yml
- filename: return-path-apps-integrations-api-openapi.yml
  format: yaml
  label: Return Path Apps & Integrations API
  slug: return-path-apps-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-apps-integrations-api-openapi.yml
- filename: return-path-certification-api-openapi.yml
  format: yaml
  label: Return Path Certification API
  slug: return-path-certification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-certification-api-openapi.yml
- filename: return-path-competitive-intel-api-openapi.yml
  format: yaml
  label: Return Path Competitive Intel API
  slug: return-path-competitive-intel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-competitive-intel-api-openapi.yml
- filename: return-path-engagement-api-openapi.yml
  format: yaml
  label: Return Path Engagement API
  slug: return-path-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-engagement-api-openapi.yml
- filename: return-path-inbox-placement-api-openapi.yml
  format: yaml
  label: Return Path Inbox Placement API
  slug: return-path-inbox-placement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-inbox-placement-api-openapi.yml
- filename: return-path-infrastructure-dmarc-api-openapi.yml
  format: yaml
  label: Return Path Infrastructure (DMARC) API
  slug: return-path-infrastructure-dmarc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-infrastructure-dmarc-api-openapi.yml
- filename: return-path-legacy-api-1-0-api-openapi.yml
  format: yaml
  label: Return Path Legacy API (1.0) API
  slug: return-path-legacy-api-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-legacy-api-1-0-api-openapi.yml
- filename: return-path-list-validation-api-openapi.yml
  format: yaml
  label: Return Path List Validation API
  slug: return-path-list-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-list-validation-api-openapi.yml
- filename: return-path-reputation-api-openapi.yml
  format: yaml
  label: Return Path Reputation API
  slug: return-path-reputation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-reputation-api-openapi.yml
- filename: return-path-view-time-optimization-api-openapi.yml
  format: yaml
  label: Return Path View Time Optimization API
  slug: return-path-view-time-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-view-time-optimization-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: returnpath.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: validity.com
  spf: true
hosts:
- cert_expires: Sep 29 12:53:58 2026 GMT
  host: www.returnpath.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 05:08:13 2026 GMT
  host: developer.everest.validity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.everest.validity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Return Path Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Return Path, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Return Path
provider_slug: return-path
slug: return-path-domain-security
source_filename: return-path-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.returnpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:53:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.everest.validity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 05:08:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.everest.validity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: returnpath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: validity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/security/return-path-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Martech
- Email
- Email Deliverability
- Email Marketing
- Sender Reputation
- Inbox Placement
- Deliverability
- DMARC
- Email Authentication
- Email Validation
- Analytics
---
