---
api_specs:
- filename: basepic-com-images-api-openapi.yml
  format: yaml
  label: BasePic Images API
  slug: basepic-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basepic-com/openapi/basepic-com-images-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:abuse@basepic.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: basepic.com
  spf: true
hosts:
- cert_expires: Dec 15 12:21:39 2026 GMT
  host: basepic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Basepic Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BasePic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BasePic
provider_slug: basepic-com
slug: basepic-com-domain-security
source_filename: basepic-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: basepic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 12:21:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: basepic.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:abuse@basepic.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/basepic-com/security/basepic-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Image Hosting
- File Sharing
- Video Hosting
- Free Service
- No Sign-up
---
