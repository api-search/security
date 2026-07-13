---
api_specs:
- filename: drupal-rest-api-openapi.yml
  format: yaml
  label: Drupal REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-rest-api-openapi.yml
- filename: drupal-jsonapi-openapi.yml
  format: yaml
  label: Drupal JSON:API
  slug: jsonapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-jsonapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: drupal.org
  spf: true
hosts:
- cert_expires: Feb 18 21:00:17 2027 GMT
  host: www.drupal.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Drupal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for drupal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: drupal
provider_slug: drupal
slug: drupal-domain-security
source_filename: drupal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drupal.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 18 21:00:17 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: drupal.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/security/drupal-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags: []
---
