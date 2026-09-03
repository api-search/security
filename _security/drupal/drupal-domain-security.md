---
api_specs:
- filename: drupal-comments-api-openapi.yml
  format: yaml
  label: drupal Comments API
  slug: drupal-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-comments-api-openapi.yml
- filename: drupal-files-api-openapi.yml
  format: yaml
  label: drupal Files API
  slug: drupal-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-files-api-openapi.yml
- filename: drupal-node-articles-api-openapi.yml
  format: yaml
  label: drupal Node Articles API
  slug: drupal-node-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-node-articles-api-openapi.yml
- filename: drupal-node-pages-api-openapi.yml
  format: yaml
  label: drupal Node Pages API
  slug: drupal-node-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-node-pages-api-openapi.yml
- filename: drupal-nodes-api-openapi.yml
  format: yaml
  label: drupal Nodes API
  slug: drupal-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-nodes-api-openapi.yml
- filename: drupal-taxonomy-terms-api-openapi.yml
  format: yaml
  label: drupal Taxonomy Terms API
  slug: drupal-taxonomy-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-taxonomy-terms-api-openapi.yml
- filename: drupal-taxonomy-vocabularies-api-openapi.yml
  format: yaml
  label: drupal Taxonomy Vocabularies API
  slug: drupal-taxonomy-vocabularies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-taxonomy-vocabularies-api-openapi.yml
- filename: drupal-users-api-openapi.yml
  format: yaml
  label: drupal Users API
  slug: drupal-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-users-api-openapi.yml
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
overview: 'Domain security posture for Drupal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Drupal
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
