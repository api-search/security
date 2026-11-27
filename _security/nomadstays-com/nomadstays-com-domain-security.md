---
api_specs:
- filename: nomadstays-com-amenities-api-openapi.yml
  format: yaml
  label: Nomad Stays Amenities API
  slug: nomadstays-com-amenities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomadstays-com/openapi/nomadstays-com-amenities-api-openapi.yml
- filename: nomadstays-com-availability-api-openapi.yml
  format: yaml
  label: Nomad Stays Availability API
  slug: nomadstays-com-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomadstays-com/openapi/nomadstays-com-availability-api-openapi.yml
- filename: nomadstays-com-health-api-openapi.yml
  format: yaml
  label: Nomad Stays Health API
  slug: nomadstays-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomadstays-com/openapi/nomadstays-com-health-api-openapi.yml
- filename: nomadstays-com-lifestyles-api-openapi.yml
  format: yaml
  label: Nomad Stays Lifestyles API
  slug: nomadstays-com-lifestyles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomadstays-com/openapi/nomadstays-com-lifestyles-api-openapi.yml
- filename: nomadstays-com-mcp-api-openapi.yml
  format: yaml
  label: Nomad Stays MCP API
  slug: nomadstays-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomadstays-com/openapi/nomadstays-com-mcp-api-openapi.yml
- filename: nomadstays-com-stays-api-openapi.yml
  format: yaml
  label: Nomad Stays Stays API
  slug: nomadstays-com-stays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomadstays-com/openapi/nomadstays-com-stays-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nomadstays.com
  spf: true
hosts:
- cert_expires: Jan 10 04:56:36 2027 GMT
  host: nomadstays.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nomad Stays Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nomad Stays, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nomad Stays
provider_slug: nomadstays-com
slug: nomadstays-com-domain-security
source_filename: nomadstays-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nomadstays.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 04:56:36 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: nomadstays.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/nomadstays-com/security/nomadstays-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Digital Nomad Accommodation
- Co-Living
- Workcation
- Travel Booking Platform
- Wi‑Fi Verified
---
