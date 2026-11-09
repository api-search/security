---
api_specs:
- filename: cyclesite-co-uk-mcp-api-api-openapi.yml
  format: yaml
  label: Cyclesite MCP API
  slug: cyclesite-co-uk-mcp-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclesite-co-uk/openapi/cyclesite-co-uk-mcp-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:t.southern@hotmail.co.uk"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cyclesite.co.uk
  spf: true
hosts:
- cert_expires: Jan 24 23:08:25 2027 GMT
  host: cyclesite.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cyclesite Co Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cyclesite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cyclesite
provider_slug: cyclesite-co-uk
slug: cyclesite-co-uk-domain-security
source_filename: cyclesite-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cyclesite.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:08:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cyclesite.co.uk\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:t.southern@hotmail.co.uk\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cyclesite-co-uk/security/cyclesite-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Bike Marketplace
- Used Bikes
- United Kingdom
- Marketplace
- Community
---
