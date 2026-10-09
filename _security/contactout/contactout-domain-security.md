---
api_specs:
- filename: contactout-openapi-generated.yml
  format: yaml
  label: ContactOut API
  slug: contactout-api-2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/_ae-authored/contactout-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: contactout.com
  spf: true
hosts:
- cert_expires: Dec  4 01:00:39 2026 GMT
  host: contactout.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contactout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ContactOut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ContactOut
provider_slug: contactout
slug: contactout-domain-security
source_filename: contactout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contactout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 01:00:39 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: contactout.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/security/contactout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Contact Data
- Email Finder
- Data Enrichment
- People Search
- Company Search
- Email Verification
- Sales Intelligence
- Recruiting
- B2B Data
---
