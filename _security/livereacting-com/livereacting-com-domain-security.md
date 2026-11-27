---
api_specs:
- filename: livereacting-com-files-api-openapi.yml
  format: yaml
  label: LiveReacting Files API
  slug: livereacting-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livereacting-com/openapi/livereacting-com-files-api-openapi.yml
- filename: livereacting-com-folders-api-openapi.yml
  format: yaml
  label: LiveReacting Folders API
  slug: livereacting-com-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livereacting-com/openapi/livereacting-com-folders-api-openapi.yml
- filename: livereacting-com-layers-api-openapi.yml
  format: yaml
  label: LiveReacting Layers API
  slug: livereacting-com-layers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livereacting-com/openapi/livereacting-com-layers-api-openapi.yml
- filename: livereacting-com-live-api-openapi.yml
  format: yaml
  label: LiveReacting Live API
  slug: livereacting-com-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livereacting-com/openapi/livereacting-com-live-api-openapi.yml
- filename: livereacting-com-playback-api-openapi.yml
  format: yaml
  label: LiveReacting Playback API
  slug: livereacting-com-playback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livereacting-com/openapi/livereacting-com-playback-api-openapi.yml
- filename: livereacting-com-projects-api-openapi.yml
  format: yaml
  label: LiveReacting Projects API
  slug: livereacting-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livereacting-com/openapi/livereacting-com-projects-api-openapi.yml
- filename: livereacting-com-scenes-api-openapi.yml
  format: yaml
  label: LiveReacting Scenes API
  slug: livereacting-com-scenes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livereacting-com/openapi/livereacting-com-scenes-api-openapi.yml
- filename: livereacting-com-streaming-destinations-api-openapi.yml
  format: yaml
  label: LiveReacting Streaming Destinations API
  slug: livereacting-com-streaming-destinations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livereacting-com/openapi/livereacting-com-streaming-destinations-api-openapi.yml
- filename: livereacting-com-system-api-openapi.yml
  format: yaml
  label: LiveReacting System API
  slug: livereacting-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livereacting-com/openapi/livereacting-com-system-api-openapi.yml
- filename: livereacting-com-workflows-api-openapi.yml
  format: yaml
  label: LiveReacting Workflows API
  slug: livereacting-com-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livereacting-com/openapi/livereacting-com-workflows-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: livereacting.com
  spf: true
hosts:
- cert_expires: Feb 15 04:35:32 2027 GMT
  host: livereacting.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LiveReacting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiveReacting, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LiveReacting
provider_slug: livereacting-com
slug: livereacting-com-domain-security
source_filename: livereacting-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: livereacting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 04:35:32 2027 GMT\n  hsts: false\ndomains:\n- domain: livereacting.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/livereacting-com/security/livereacting-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Live Streaming
- Interactive
- Artificial Intelligence
- Video
- Software-as-a-Service
---
