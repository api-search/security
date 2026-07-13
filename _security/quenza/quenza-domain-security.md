---
api_specs:
- filename: quenza-openapi.yml
  format: yaml
  label: Quenza Clients API
  slug: quenza-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-openapi.yml
- filename: quenza-openapi.yml
  format: yaml
  label: Quenza Groups API
  slug: quenza-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-openapi.yml
- filename: quenza-openapi.yml
  format: yaml
  label: Quenza Members API
  slug: quenza-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-openapi.yml
- filename: quenza-openapi.yml
  format: yaml
  label: Quenza Tasks API
  slug: quenza-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quenza.com
  spf: true
hosts:
- cert_expires: Aug 17 18:32:49 2026 GMT
  host: quenza.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 22:47:47 2026 GMT
  host: developers.quenza.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quenza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quenza, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quenza
provider_slug: quenza
slug: quenza-domain-security
source_filename: quenza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quenza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 18:32:49 2026 GMT\n  hsts: false\n- host: developers.quenza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:47:47 2026 GMT\n  hsts: false\ndomains:\n- domain: quenza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/security/quenza-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Coaching
- Therapy
- Client Engagement
- Digital Health
- Mental Health
- Practice Management
- Positive Psychology
---
