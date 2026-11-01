---
api_specs:
- filename: mcp-tools.json
  format: json
  label: Valuation API
  slug: valuation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ascent-partners-com/openapi/mcp-tools.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ascent-partners.com
  spf: true
hosts:
- cert_expires: Jan 11 03:55:53 2027 GMT
  host: ascent-partners.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ascent Partners Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ascent-partners-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ascent-partners-com
provider_slug: ascent-partners-com
slug: ascent-partners-com-domain-security
source_filename: ascent-partners-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ascent-partners.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 03:55:53 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ascent-partners.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ascent-partners-com/security/ascent-partners-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Valuation
- Advisory
- Finance
- Technology
- Asia
---
