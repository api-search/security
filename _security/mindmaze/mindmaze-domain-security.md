---
api_specs:
- filename: mindmaze-discovery-api-openapi.yml
  format: yaml
  label: MindMaze Discovery API
  slug: mindmaze-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-discovery-api-openapi.yml
- filename: mindmaze-media-api-openapi.yml
  format: yaml
  label: MindMaze Media API
  slug: mindmaze-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-media-api-openapi.yml
- filename: mindmaze-oembed-api-openapi.yml
  format: yaml
  label: MindMaze O Embed API
  slug: mindmaze-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-oembed-api-openapi.yml
- filename: mindmaze-pages-api-openapi.yml
  format: yaml
  label: MindMaze Pages API
  slug: mindmaze-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-pages-api-openapi.yml
- filename: mindmaze-posts-api-openapi.yml
  format: yaml
  label: MindMaze Posts API
  slug: mindmaze-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-posts-api-openapi.yml
- filename: mindmaze-search-api-openapi.yml
  format: yaml
  label: MindMaze Search API
  slug: mindmaze-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-search-api-openapi.yml
- filename: mindmaze-taxonomy-api-openapi.yml
  format: yaml
  label: MindMaze Taxonomy API
  slug: mindmaze-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mindmazetherapeutics.com
  spf: true
hosts:
- cert_expires: Sep 18 19:53:06 2026 GMT
  host: mindmazetherapeutics.com
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mindmaze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MindMaze, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MindMaze
provider_slug: mindmaze
slug: mindmaze-domain-security
source_filename: mindmaze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mindmazetherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 19:53:06 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: mindmazetherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/security/mindmaze-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Therapeutics
- Neurotechnology
- Neurorehabilitation
- Medical Devices
- Health
- Artificial Intelligence
- Stroke
- Parkinsons Disease
- Switzerland
---
