---
api_specs:
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Video Generation API
  slug: video-generation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Avatars / Presenters API
  slug: avatars-presenters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Job Status / Webhooks API
  slug: job-status-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: colossyan.com
  spf: true
hosts:
- cert_expires: Oct  4 14:15:45 2026 GMT
  host: www.colossyan.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 19:12:25 2026 GMT
  host: docs.colossyan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 15:39:33 2026 GMT
  host: app.colossyan.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Colossyan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Colossyan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Colossyan
provider_slug: colossyan
slug: colossyan-domain-security
source_filename: colossyan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.colossyan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:15:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.colossyan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:12:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.colossyan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 15:39:33 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: colossyan.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/security/colossyan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Video Generation
- Avatars
- Text to Video
- Learning and Development
---
