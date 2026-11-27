---
api_specs:
- filename: kaneme-com-certificat-api-openapi.yml
  format: yaml
  label: Kaneme Certificat API
  slug: kaneme-com-certificat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-certificat-api-openapi.yml
- filename: kaneme-com-compte-api-openapi.yml
  format: yaml
  label: Kaneme Compte API
  slug: kaneme-com-compte-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-compte-api-openapi.yml
- filename: kaneme-com-criture-api-openapi.yml
  format: yaml
  label: Kaneme Écriture API
  slug: kaneme-com-criture-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-criture-api-openapi.yml
- filename: kaneme-com-cycle-de-vie-api-openapi.yml
  format: yaml
  label: Kaneme Cycle de vie API
  slug: kaneme-com-cycle-de-vie-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-cycle-de-vie-api-openapi.yml
- filename: kaneme-com-documents-api-openapi.yml
  format: yaml
  label: Kaneme Documents API
  slug: kaneme-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-documents-api-openapi.yml
- filename: kaneme-com-mesure-api-openapi.yml
  format: yaml
  label: Kaneme Mesure API
  slug: kaneme-com-mesure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-mesure-api-openapi.yml
- filename: kaneme-com-projets-api-openapi.yml
  format: yaml
  label: Kaneme Projets API
  slug: kaneme-com-projets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-projets-api-openapi.yml
- filename: kaneme-com-voix-api-openapi.yml
  format: yaml
  label: Kaneme Voix API
  slug: kaneme-com-voix-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-voix-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kaneme.com
  spf: true
hosts:
- cert_expires: Jan  7 18:00:55 2027 GMT
  host: kaneme.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kaneme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaneme, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kaneme
provider_slug: kaneme-com
slug: kaneme-com-domain-security
source_filename: kaneme-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kaneme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 18:00:55 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kaneme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kaneme-com/security/kaneme-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Voice
- Personalization
---
