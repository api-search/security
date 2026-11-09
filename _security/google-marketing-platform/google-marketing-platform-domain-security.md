---
api_specs:
- filename: google-marketing-platform-v1alpha-api-openapi.yml
  format: yaml
  label: Google Marketing Platform Admin V1alpha API
  slug: google-marketing-platform-v1alpha-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-marketing-platform/openapi/google-marketing-platform-v1alpha-api-openapi.yml
- filename: google-marketing-platform-adminaccessbindings-api-openapi.yml
  format: yaml
  label: Google Marketing Platform Admin Admin Access Bindings API
  slug: google-marketing-platform-adminaccessbindings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-marketing-platform/openapi/google-marketing-platform-adminaccessbindings-api-openapi.yml
- filename: google-marketing-platform-analyticsaccountlinks-api-openapi.yml
  format: yaml
  label: Google Marketing Platform Admin Analytics Account Links API
  slug: google-marketing-platform-analyticsaccountlinks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-marketing-platform/openapi/google-marketing-platform-analyticsaccountlinks-api-openapi.yml
- filename: google-marketing-platform-members-api-openapi.yml
  format: yaml
  label: Google Marketing Platform Admin Members API
  slug: google-marketing-platform-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-marketing-platform/openapi/google-marketing-platform-members-api-openapi.yml
- filename: google-marketing-platform-organizations-api-openapi.yml
  format: yaml
  label: Google Marketing Platform Admin Organizations API
  slug: google-marketing-platform-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-marketing-platform/openapi/google-marketing-platform-organizations-api-openapi.yml
- filename: google-marketing-platform-user-groups-api-openapi.yml
  format: yaml
  label: Google Marketing Platform Admin User Groups API
  slug: google-marketing-platform-user-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-marketing-platform/openapi/google-marketing-platform-user-groups-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Dec 30 19:09:53 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: marketingplatform.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Marketing Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Marketing Platform Admin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Marketing Platform Admin
provider_slug: google-marketing-platform
slug: google-marketing-platform-domain-security
source_filename: google-marketing-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: marketingplatform.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: false\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-marketing-platform/security/google-marketing-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Google Marketing Platform
- Marketing
- Organization Management
- Platform Administration
---
