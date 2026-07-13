---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Imgflip Meme Generator API
  slug: imgflip-meme-generator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imgflip/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: imgflip.com
  spf: true
hosts:
- cert_expires: Oct  3 01:45:52 2026 GMT
  host: imgflip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 01:45:52 2026 GMT
  host: api.imgflip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imgflip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imgflip, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Imgflip
provider_slug: imgflip
slug: imgflip-domain-security
source_filename: imgflip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imgflip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:45:52 2026 GMT\n  hsts: false\n- host: api.imgflip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:45:52 2026 GMT\n  hsts: false\ndomains:\n- domain: imgflip.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imgflip/refs/heads/main/security/imgflip-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Memes
- Images
- GIFs
- Entertainment
- AI
- Image Generation
---
