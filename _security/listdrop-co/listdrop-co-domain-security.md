---
api_specs:
- filename: listdrop-co-discovery-api-openapi.yml
  format: yaml
  label: ListDrop Discovery API
  slug: listdrop-co-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-discovery-api-openapi.yml
- filename: listdrop-co-feedback-api-openapi.yml
  format: yaml
  label: ListDrop Feedback API
  slug: listdrop-co-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-feedback-api-openapi.yml
- filename: listdrop-co-lists-api-openapi.yml
  format: yaml
  label: ListDrop Lists API
  slug: listdrop-co-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-lists-api-openapi.yml
- filename: listdrop-co-read-api-openapi.yml
  format: yaml
  label: ListDrop Read API
  slug: listdrop-co-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-read-api-openapi.yml
- filename: listdrop-co-webhooks-api-openapi.yml
  format: yaml
  label: ListDrop Webhooks API
  slug: listdrop-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: listdrop.co
  spf: true
hosts:
- cert_expires: Feb 14 23:51:14 2027 GMT
  host: listdrop.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ListDrop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ListDrop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ListDrop
provider_slug: listdrop-co
slug: listdrop-co-domain-security
source_filename: listdrop-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: listdrop.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:51:14 2027 GMT\n  hsts: false\ndomains:\n- domain: listdrop.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/listdrop-co/security/listdrop-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social
- List
- Community
- Artificial Intelligence
- Platform
---
