---
api_specs:
- filename: stanley-black-and-decker-tool-connect-api-openapi.yml
  format: yaml
  label: DEWALT Tool Connect API
  slug: dewalt-tool-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanley-black-and-decker/refs/heads/main/openapi/stanley-black-and-decker-tool-connect-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stanleyblackanddecker.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dewalt.com
  spf: true
hosts:
- cert_expires: Jul 16 08:49:42 2026 GMT
  host: www.stanleyblackanddecker.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 13:16:47 2026 GMT
  host: www.dewalt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: developer.stanley.com
  https: false
kind: domain-security
layout: security
method: probed
name: Stanley Black And Decker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stanley Black & Decker, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stanley Black & Decker
provider_slug: stanley-black-and-decker
slug: stanley-black-and-decker-domain-security
source_filename: stanley-black-and-decker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stanleyblackanddecker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 16 08:49:42 2026 GMT\n  hsts: null\n- host: www.dewalt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 13:16:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.stanley.com\n  https: false\ndomains:\n- domain: stanleyblackanddecker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dewalt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stanley-black-and-decker/refs/heads/main/security/stanley-black-and-decker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tools
- Hardware
- Manufacturing
- IoT
- Connected Tools
- Fortune 500
---
