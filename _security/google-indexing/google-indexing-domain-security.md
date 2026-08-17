---
api_specs:
- filename: google-indexing-urlnotifications-api-openapi.yml
  format: yaml
  label: Google Indexing urlNotifications API
  slug: google-indexing-urlnotifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-indexing/refs/heads/main/openapi/google-indexing-urlnotifications-api-openapi.yml
- filename: google-indexing-urlnotifications-publish-api-openapi.yml
  format: yaml
  label: Google Indexing urlNotifications:publish API
  slug: google-indexing-urlnotifications-publish-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-indexing/refs/heads/main/openapi/google-indexing-urlnotifications-publish-api-openapi.yml
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
- cert_expires: Oct 12 18:05:55 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:07:34 2026 GMT
  host: indexing.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Indexing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Indexing, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Indexing
provider_slug: google-indexing
slug: google-indexing-domain-security
source_filename: google-indexing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:05:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: indexing.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:07:34 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-indexing/refs/heads/main/security/google-indexing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Crawling
- Google
- Indexing
- Search
- SEO
- URLs
---
