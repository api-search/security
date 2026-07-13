---
api_specs:
- filename: contentful-openapi.yml
  format: yaml
  label: Contentful Content Delivery API
  slug: contentful-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentful/refs/heads/main/openapi/contentful-openapi.yml
- filename: contentful-webhooks-asyncapi.yml
  format: yaml
  label: Contentful Webhooks
  slug: contentful-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentful/refs/heads/main/openapi/contentful-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: contentful.com
  spf: true
hosts:
- cert_expires: Sep 22 13:18:24 2026 GMT
  host: www.contentful.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:00:19 2027 GMT
  host: cdn.contentful.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Contentful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contentful, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Contentful
provider_slug: contentful
slug: contentful-domain-security
source_filename: contentful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.contentful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:18:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cdn.contentful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:00:19 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: contentful.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contentful/refs/heads/main/security/contentful-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content
---
