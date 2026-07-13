---
api_specs:
- filename: add-captions-to-a-video
  format: yaml
  label: Captions Video Captions API
  slug: captions-ai-video-captions-api
  spec_type: OpenAPI
  url: https://captions.ai/help/api-reference/video-captions/add-captions-to-a-video
- filename: captions-ai-creator-ads-openapi.yml
  format: yaml
  label: Captions AI Creator API
  slug: captions-ai-creator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions-ai/refs/heads/main/openapi/captions-ai-creator-ads-openapi.yml
- filename: captions-ai-creator-ads-openapi.yml
  format: yaml
  label: Captions AI Ads API
  slug: captions-ai-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions-ai/refs/heads/main/openapi/captions-ai-creator-ads-openapi.yml
- filename: captions-ai-mirage-video-openapi.yml
  format: yaml
  label: Mirage Video Generation API
  slug: captions-mirage-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions-ai/refs/heads/main/openapi/captions-ai-mirage-video-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: captions.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mirage.app
  spf: true
hosts:
- cert_expires: Sep  2 20:35:07 2026 GMT
  host: captions.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 16:44:58 2026 GMT
  host: api.mirage.app
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 15:26:20 2026 GMT
  host: api.captions.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Captions Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Captions, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Captions
provider_slug: captions-ai
slug: captions-ai-domain-security
source_filename: captions-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: captions.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:35:07 2026 GMT\n  hsts: false\n- host: api.mirage.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:44:58 2026 GMT\n  hsts: null\n- host: api.captions.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:26:20 2026 GMT\n  hsts: null\ndomains:\n- domain: captions.ai\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mirage.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captions-ai/refs/heads/main/security/captions-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- AI Video
- Video Generation
- Video Captioning
- AI Dubbing
- Lip Sync
- AI Twin
- Text to Video
- Generative AI
- Video Translation
---
