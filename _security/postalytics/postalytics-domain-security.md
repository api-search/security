---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Postalytics API
  slug: postalytics-api
  spec_type: OpenAPI
  url: https://docs.postalytics.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: postalytics.com
  spf: true
hosts:
- cert_expires: Sep 10 14:24:52 2026 GMT
  host: www.postalytics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 01:37:47 2026 GMT
  host: api.postalytics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postalytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Postalytics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Postalytics
provider_slug: postalytics
slug: postalytics-domain-security
source_filename: postalytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.postalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:24:52 2026 GMT\n  hsts: false\n- host: api.postalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 01:37:47 2026 GMT\n  hsts: null\ndomains:\n- domain: postalytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postalytics/refs/heads/main/security/postalytics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Direct Mail
- Postcards
- Letters
- Mail Automation
- Print
- Tracking
- Analytics
---
