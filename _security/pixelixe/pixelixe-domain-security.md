---
api_specs:
- filename: pixelixe-openapi.yml
  format: yaml
  label: Pixelixe
  slug: pixelixe
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelixe/refs/heads/main/openapi/pixelixe-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pixelixe.com
  spf: true
hosts:
- cert_expires: Aug 28 04:46:57 2026 GMT
  host: pixelixe.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 23:19:02 2026 GMT
  host: studio.pixelixe.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixelixe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixelixe, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Pixelixe
provider_slug: pixelixe
slug: pixelixe-domain-security
source_filename: pixelixe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pixelixe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 04:46:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: studio.pixelixe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:19:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: pixelixe.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixelixe/refs/heads/main/security/pixelixe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Graphics
- Images
---
