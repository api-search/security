---
api_specs:
- filename: google-books-volumes-api-openapi.yml
  format: yaml
  label: Google Books Volumes API
  slug: google-books-volumes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-volumes-api-openapi.yml
- filename: google-books-bookshelves-api-openapi.yml
  format: yaml
  label: Google Books Bookshelves API
  slug: google-books-bookshelves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-bookshelves-api-openapi.yml
- filename: google-books-cloudloading-api-openapi.yml
  format: yaml
  label: Google Books Cloudloading API
  slug: google-books-cloudloading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-cloudloading-api-openapi.yml
- filename: google-books-dictionary-api-openapi.yml
  format: yaml
  label: Google Books Dictionary API
  slug: google-books-dictionary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-dictionary-api-openapi.yml
- filename: google-books-familysharing-api-openapi.yml
  format: yaml
  label: Google Books Familysharing API
  slug: google-books-familysharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-familysharing-api-openapi.yml
- filename: google-books-layers-api-openapi.yml
  format: yaml
  label: Google Books Layers API
  slug: google-books-layers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-layers-api-openapi.yml
- filename: google-books-myconfig-api-openapi.yml
  format: yaml
  label: Google Books Myconfig API
  slug: google-books-myconfig-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-myconfig-api-openapi.yml
- filename: google-books-notification-api-openapi.yml
  format: yaml
  label: Google Books Notification API
  slug: google-books-notification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-notification-api-openapi.yml
- filename: google-books-onboarding-api-openapi.yml
  format: yaml
  label: Google Books Onboarding API
  slug: google-books-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-onboarding-api-openapi.yml
- filename: google-books-personalizedstream-api-openapi.yml
  format: yaml
  label: Google Books Personalizedstream API
  slug: google-books-personalizedstream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-personalizedstream-api-openapi.yml
- filename: google-books-promooffer-api-openapi.yml
  format: yaml
  label: Google Books Promooffer API
  slug: google-books-promooffer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-promooffer-api-openapi.yml
- filename: google-books-series-api-openapi.yml
  format: yaml
  label: Google Books Series API
  slug: google-books-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-series-api-openapi.yml
- filename: google-books-mylibrary-api-openapi.yml
  format: yaml
  label: Google Books Books Mylibrary API
  slug: google-books-mylibrary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-mylibrary-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Dec 30 19:09:53 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: www.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Books Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Books, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Books
provider_slug: google-books
slug: google-books-domain-security
source_filename: google-books-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-books/security/google-books-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Books
- Ebooks
- Google
- Library
- Publishing
- Reading
- Search
---
