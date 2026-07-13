---
api_specs:
- filename: picpurify-openapi.yaml
  format: yaml
  label: PicPurify Moderation API
  slug: picpurify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picpurify/refs/heads/main/openapi/picpurify-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: picpurify.com
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.picpurify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Picpurify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PicPurify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PicPurify
provider_slug: picpurify
slug: picpurify-domain-security
source_filename: picpurify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.picpurify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: picpurify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picpurify/refs/heads/main/security/picpurify-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Image Moderation
- Content Moderation
- Computer Vision
- Weapon Detection
---
