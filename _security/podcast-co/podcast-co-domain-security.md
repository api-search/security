---
api_specs:
- filename: podcast-co-episodes-api-openapi.yml
  format: yaml
  label: Podcast.co Episodes API
  slug: podcast-co-episodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podcast-co/openapi/podcast-co-episodes-api-openapi.yml
- filename: podcast-co-podcast-page-api-openapi.yml
  format: yaml
  label: Podcast.co podcast page API
  slug: podcast-co-podcast-page-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podcast-co/openapi/podcast-co-podcast-page-api-openapi.yml
- filename: podcast-co-podcasts-api-openapi.yml
  format: yaml
  label: Podcast.co Podcasts API
  slug: podcast-co-podcasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podcast-co/openapi/podcast-co-podcasts-api-openapi.yml
- filename: podcast-co-subscribe-button-api-openapi.yml
  format: yaml
  label: Podcast.co subscribe button API
  slug: podcast-co-subscribe-button-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podcast-co/openapi/podcast-co-subscribe-button-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: podcast.co
  spf: true
hosts:
- cert_expires: Jan  9 06:55:17 2027 GMT
  host: podcast.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Podcast Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Podcast.co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Podcast.co
provider_slug: podcast-co
slug: podcast-co-domain-security
source_filename: podcast-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: podcast.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 06:55:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: podcast.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/podcast-co/security/podcast-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Podcasting
- Hosting
- Audio
- SaaS
- Media
---
