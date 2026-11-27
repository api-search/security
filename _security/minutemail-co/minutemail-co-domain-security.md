---
api_specs:
- filename: minutemail-co-openapi-generated.yml
  format: yaml
  label: MinuteMail API
  slug: minutemail-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minutemail-co/openapi/_ae-authored/minutemail-co-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: minutemail.co
  spf: true
hosts:
- cert_expires: Jan 16 12:34:36 2027 GMT
  host: minutemail.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MinuteMail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MinuteMail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MinuteMail
provider_slug: minutemail-co
slug: minutemail-co-domain-security
source_filename: minutemail-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: minutemail.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 12:34:36 2027 GMT\n  hsts: false\ndomains:\n- domain: minutemail.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/minutemail-co/security/minutemail-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email Testing
- Auth Testing
- Mock OAuth
- REST API
- SDK
- MCP Server
- Ephemeral Mailboxes
---
