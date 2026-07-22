---
api_specs:
- filename: skymerse-notamify-openapi-original.json
  format: json
  label: Notamify API V2
  slug: notamify-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skymerse/refs/heads/main/openapi/skymerse-notamify-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: notamify.com
  spf: true
hosts:
- cert_expires: Oct 17 12:48:37 2026 GMT
  host: api.notamify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skymerse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skymerse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Skymerse
provider_slug: skymerse
slug: skymerse-domain-security
source_filename: skymerse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.notamify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 12:48:37 2026 GMT\n  hsts: null\ndomains:\n- domain: notamify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skymerse/refs/heads/main/security/skymerse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aviation
- NOTAM
- Flight Operations
- Aeronautical
- Weather
- AI
- Webhooks
---
