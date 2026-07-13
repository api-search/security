---
api_specs:
- filename: adobe-premiere-creative-cloud-libraries-openapi.yml
  format: yaml
  label: Adobe Creative Cloud Libraries API
  slug: adobe-creative-cloud-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/openapi/adobe-premiere-creative-cloud-libraries-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.io
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.adobe.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: api.adobe.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: cc-libraries.adobe.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adobe Premiere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Premiere Pro, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Premiere Pro
provider_slug: adobe-premiere
slug: adobe-premiere-domain-security
source_filename: adobe-premiere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\n- host: cc-libraries.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adobe.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/security/adobe-premiere-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Adobe
- Automation
- Creative Cloud
- Media
- Premiere Pro
- Video Editing
- Video Production
---
