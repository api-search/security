---
api_specs:
- filename: anahana-com-discovery-api-openapi.yml
  format: yaml
  label: Anahana Discovery API
  slug: anahana-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anahana-com/openapi/anahana-com-discovery-api-openapi.yml
- filename: anahana-com-mcp-api-openapi.yml
  format: yaml
  label: Anahana MCP API
  slug: anahana-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anahana-com/openapi/anahana-com-mcp-api-openapi.yml
- filename: anahana-com-oauth-api-openapi.yml
  format: yaml
  label: Anahana OAuth API
  slug: anahana-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anahana-com/openapi/anahana-com-oauth-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: anahana.com
  spf: true
hosts:
- cert_expires: Jan 19 10:45:34 2027 GMT
  host: anahana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anahana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anahana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Anahana
provider_slug: anahana-com
slug: anahana-com-domain-security
source_filename: anahana-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anahana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 10:45:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anahana.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/anahana-com/security/anahana-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- SpiritualWellness
- Personal Growth
- Astrology
- Meditation
- Yoga
---
