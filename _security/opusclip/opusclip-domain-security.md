---
api_specs:
- filename: opusclip-brand-templates-api-openapi.yml
  format: yaml
  label: OpusClip brand-templates API
  slug: opusclip-brand-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-brand-templates-api-openapi.yml
- filename: opusclip-censor-jobs-api-openapi.yml
  format: yaml
  label: OpusClip censor-jobs API
  slug: opusclip-censor-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-censor-jobs-api-openapi.yml
- filename: opusclip-clip-project-api-openapi.yml
  format: yaml
  label: OpusClip clip-project API
  slug: opusclip-clip-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-clip-project-api-openapi.yml
- filename: opusclip-collection-api-openapi.yml
  format: yaml
  label: OpusClip collection API
  slug: opusclip-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-collection-api-openapi.yml
- filename: opusclip-collection-content-api-openapi.yml
  format: yaml
  label: OpusClip collection-content API
  slug: opusclip-collection-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-collection-content-api-openapi.yml
- filename: opusclip-enterprise-api-openapi.yml
  format: yaml
  label: OpusClip enterprise API
  slug: opusclip-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-enterprise-api-openapi.yml
- filename: opusclip-exportable-clips-api-openapi.yml
  format: yaml
  label: OpusClip exportable-clips API
  slug: opusclip-exportable-clips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-exportable-clips-api-openapi.yml
- filename: opusclip-exportableclip-api-openapi.yml
  format: yaml
  label: OpusClip ExportableClip API
  slug: opusclip-exportableclip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-exportableclip-api-openapi.yml
- filename: opusclip-generative-jobs-api-openapi.yml
  format: yaml
  label: OpusClip generative-jobs API
  slug: opusclip-generative-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-generative-jobs-api-openapi.yml
- filename: opusclip-social-posting-api-openapi.yml
  format: yaml
  label: OpusClip social-posting API
  slug: opusclip-social-posting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-social-posting-api-openapi.yml
- filename: opusclip-transcripts-api-openapi.yml
  format: yaml
  label: OpusClip transcripts API
  slug: opusclip-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-transcripts-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: opus.pro
  spf: true
hosts:
- cert_expires: Aug 22 18:01:23 2026 GMT
  host: api.opus.pro
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opusclip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpusClip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OpusClip
provider_slug: opusclip
slug: opusclip-domain-security
source_filename: opusclip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.opus.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 18:01:23 2026 GMT\n  hsts: false\ndomains:\n- domain: opus.pro\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/security/opusclip-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Video
- AI
- Video Editing
- Short-Form Video
- Social Media
- Content Creation
- MCP
- Developer API
---
