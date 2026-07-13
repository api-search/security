---
api_specs:
- filename: magento-rest-api-openapi.yml
  format: yaml
  label: Magento REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-rest-api-openapi.yml
- filename: magento-webhooks-asyncapi.yml
  format: yaml
  label: Adobe Commerce Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/asyncapi/magento-webhooks-asyncapi.yml
- filename: magento-events-asyncapi.yml
  format: yaml
  label: Adobe Commerce Eventing
  slug: events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/asyncapi/magento-events-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.adobe.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Magento Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for magento, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: magento
provider_slug: magento
slug: magento-domain-security
source_filename: magento-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/security/magento-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags: []
---
