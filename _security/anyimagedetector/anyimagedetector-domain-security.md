---
api_specs:
- filename: anyimagedetector-ai-image-detector-openapi.yml
  format: yaml
  label: AI Image Detector API
  slug: ai-image-detector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anyimagedetector/refs/heads/main/openapi/anyimagedetector-ai-image-detector-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: imagedetector.online
  spf: true
hosts:
- cert_expires: Oct 15 13:26:38 2026 GMT
  host: imagedetector.online
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anyimagedetector Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AnyImageDetector, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AnyImageDetector
provider_slug: anyimagedetector
slug: anyimagedetector-domain-security
source_filename: anyimagedetector-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imagedetector.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 13:26:38 2026 GMT\n  hsts: false\ndomains:\n- domain: imagedetector.online\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anyimagedetector/refs/heads/main/security/anyimagedetector-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI image detection
- Image Analysis
- Computer-Vision
- Content Moderation
- Trust and Safety
- Fact Checking
- media verification
- Developer Tools
- Synthetic Media
- Fraud Prevention
---
