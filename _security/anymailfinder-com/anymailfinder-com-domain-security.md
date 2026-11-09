---
api_specs:
- filename: anymailfinder-com-account-api-openapi.yml
  format: yaml
  label: Anymail Finder Account API
  slug: anymailfinder-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-account-api-openapi.yml
- filename: anymailfinder-com-bulk-api-openapi.yml
  format: yaml
  label: Anymail Finder Bulk API
  slug: anymailfinder-com-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-bulk-api-openapi.yml
- filename: anymailfinder-com-domain-api-openapi.yml
  format: yaml
  label: Anymail Finder Domain API
  slug: anymailfinder-com-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-domain-api-openapi.yml
- filename: anymailfinder-com-find-email-api-openapi.yml
  format: yaml
  label: Anymail Finder Find Email API
  slug: anymailfinder-com-find-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-find-email-api-openapi.yml
- filename: anymailfinder-com-geo-lead-api-openapi.yml
  format: yaml
  label: Anymail Finder Geo Lead API
  slug: anymailfinder-com-geo-lead-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-geo-lead-api-openapi.yml
- filename: anymailfinder-com-report-api-openapi.yml
  format: yaml
  label: Anymail Finder Report API
  slug: anymailfinder-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-report-api-openapi.yml
- filename: anymailfinder-com-verify-email-api-openapi.yml
  format: yaml
  label: Anymail Finder Verify Email API
  slug: anymailfinder-com-verify-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-verify-email-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anymailfinder.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: anymailfinder.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anymailfinder Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anymail Finder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Anymail Finder
provider_slug: anymailfinder-com
slug: anymailfinder-com-domain-security
source_filename: anymailfinder-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anymailfinder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: anymailfinder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/anymailfinder-com/security/anymailfinder-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Finder
- B2B
- Lead Generation
- Verification
---
