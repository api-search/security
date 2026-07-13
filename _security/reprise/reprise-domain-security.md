---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Reprise Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://docs.reprise.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: reprise.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zendesk.com
  spf: true
hosts:
- cert_expires: Sep  7 21:48:38 2026 GMT
  host: www.reprise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.reprise.com
  https: false
- cert_expires: Sep  1 00:04:20 2026 GMT
  host: reprise.zendesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reprise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reprise, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Reprise
provider_slug: reprise
slug: reprise-domain-security
source_filename: reprise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reprise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:48:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.reprise.com\n  https: false\n- host: reprise.zendesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:04:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reprise.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: zendesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reprise/refs/heads/main/security/reprise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Demo Automation
- Product Tours
- Sales Demos
- Interactive Demos
- Sandbox Environments
- Enterprise Sales
- Marketing Technology
- Sales Enablement
---
