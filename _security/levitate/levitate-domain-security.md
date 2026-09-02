---
api_specs:
- filename: levitate-companies-api-openapi.yml
  format: yaml
  label: Levitate Companies API
  slug: levitate-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levitate/refs/heads/main/openapi/levitate-companies-api-openapi.yml
- filename: levitate-contacts-api-openapi.yml
  format: yaml
  label: Levitate Contacts API
  slug: levitate-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levitate/refs/heads/main/openapi/levitate-contacts-api-openapi.yml
- filename: levitate-notes-api-openapi.yml
  format: yaml
  label: Levitate Notes API
  slug: levitate-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levitate/refs/heads/main/openapi/levitate-notes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: levitate.ai
  spf: false
- caa: []
  dmarc: true
  dmarc_record: v=DMARC1; p=none;
  dnssec: false
  domain: levitateapp.com
  note: Levitate's corporate/sending and security-contact domain (security@levitateapp.com). Added by hand from a direct dig; the probe script only walks hosts named in apis.yml, which all sit on levitate.ai.
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:helpscoutemail.com include:_spf.sendergen.com ~all
hosts:
- cert_expires: Nov  8 07:57:47 2026 GMT
  host: www.levitate.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:24:50 2026 GMT
  host: help.levitate.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: api.levitate.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Levitate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Levitate, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Levitate
provider_slug: levitate
slug: levitate-domain-security
source_filename: levitate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.levitate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 07:57:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.levitate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:24:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.levitate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: levitate.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: levitateapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:helpscoutemail.com include:_spf.sendergen.com ~all\n  dmarc: true\n  dmarc_record: v=DMARC1; p=none;\n  note: Levitate's corporate/sending and security-contact domain (security@levitateapp.com). Added by\n    hand from a direct dig; the probe script only\
  \ walks hosts named in apis.yml, which all sit on levitate.ai.\nnote: \"levitate.ai itself publishes no SPF, DMARC, CAA or DNSSEC records (verified by dig 2026-08-25)\\\n  \\ \\u2014 notable for an email-marketing vendor. The sending and corporate domain levitateapp.com does\\\n  \\ publish SPF and DMARC, but DMARC is at p=none (monitor only, no enforcement). api.levitate.ai serves\\\n  \\ no HSTS header; www.levitate.ai and help.levitate.ai do, at max-age=31536000.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levitate/refs/heads/main/security/levitate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- relationship-marketing
- CRM
- Email Marketing
- Contacts
- Small Business
- Insurance
- Financial-Services
- Non-Profit
- Marketing Automation
- MCP
- agent-native
- Software-as-a-Service
---
