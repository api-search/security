---
api_specs:
- filename: radio-mast-openapi.yml
  format: yaml
  label: Radio Mast
  slug: radio-mast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radio-mast/refs/heads/main/openapi/radio-mast-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: radiomast.io
  spf: true
hosts:
- cert_expires: Sep 11 20:23:13 2026 GMT
  host: www.radiomast.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 12 14:07:21 2026 GMT
  host: api.radiomast.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Radio Mast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Radio Mast, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Radio Mast
provider_slug: radio-mast
slug: radio-mast-domain-security
source_filename: radio-mast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.radiomast.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 20:23:13 2026 GMT\n  hsts: false\n- host: api.radiomast.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 12 14:07:21 2026 GMT\n  hsts: false\ndomains:\n- domain: radiomast.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radio-mast/refs/heads/main/security/radio-mast-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Radio
- Streaming
- Analytics
- Audio
- Broadcasting
---
