---
api_specs:
- filename: ki-alternativen-com-agents-md-api-openapi.yml
  format: yaml
  label: KI Alternativen AGENTS.md API
  slug: ki-alternativen-com-agents-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ki-alternativen-com/openapi/ki-alternativen-com-agents-md-api-openapi.yml
- filename: ki-alternativen-com-auth-md-api-openapi.yml
  format: yaml
  label: KI Alternativen Auth.md API
  slug: ki-alternativen-com-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ki-alternativen-com/openapi/ki-alternativen-com-auth-md-api-openapi.yml
- filename: ki-alternativen-com-llms-full-txt-api-openapi.yml
  format: yaml
  label: KI Alternativen Llms Full.txt API
  slug: ki-alternativen-com-llms-full-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ki-alternativen-com/openapi/ki-alternativen-com-llms-full-txt-api-openapi.yml
- filename: ki-alternativen-com-llms-txt-api-openapi.yml
  format: yaml
  label: KI Alternativen Llms.txt API
  slug: ki-alternativen-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ki-alternativen-com/openapi/ki-alternativen-com-llms-txt-api-openapi.yml
- filename: ki-alternativen-com-openapi-json-api-openapi.yml
  format: yaml
  label: KI Alternativen Openapi.json API
  slug: ki-alternativen-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ki-alternativen-com/openapi/ki-alternativen-com-openapi-json-api-openapi.yml
- filename: ki-alternativen-com-pricing-md-api-openapi.yml
  format: yaml
  label: KI Alternativen Pricing.md API
  slug: ki-alternativen-com-pricing-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ki-alternativen-com/openapi/ki-alternativen-com-pricing-md-api-openapi.yml
- filename: ki-alternativen-com-robots-txt-api-openapi.yml
  format: yaml
  label: KI Alternativen Robots.txt API
  slug: ki-alternativen-com-robots-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ki-alternativen-com/openapi/ki-alternativen-com-robots-txt-api-openapi.yml
- filename: ki-alternativen-com-server-json-api-openapi.yml
  format: yaml
  label: KI Alternativen Server.json API
  slug: ki-alternativen-com-server-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ki-alternativen-com/openapi/ki-alternativen-com-server-json-api-openapi.yml
- filename: ki-alternativen-com-sitemap-md-api-openapi.yml
  format: yaml
  label: KI Alternativen Sitemap.md API
  slug: ki-alternativen-com-sitemap-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ki-alternativen-com/openapi/ki-alternativen-com-sitemap-md-api-openapi.yml
- filename: ki-alternativen-com-sitemap-xml-api-openapi.yml
  format: yaml
  label: KI Alternativen Sitemap.xml API
  slug: ki-alternativen-com-sitemap-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ki-alternativen-com/openapi/ki-alternativen-com-sitemap-xml-api-openapi.yml
- filename: ki-alternativen-com-well-known-api-openapi.yml
  format: yaml
  label: KI Alternativen .well Known API
  slug: ki-alternativen-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ki-alternativen-com/openapi/ki-alternativen-com-well-known-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ki-alternativen.com
  spf: true
hosts:
- cert_expires: Jan 26 15:05:45 2027 GMT
  host: ki-alternativen.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KI Alternativen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KI Alternativen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KI Alternativen
provider_slug: ki-alternativen-com
slug: ki-alternativen-com-domain-security
source_filename: ki-alternativen-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ki-alternativen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 15:05:45 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ki-alternativen.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ki-alternativen-com/security/ki-alternativen-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Tools
- Directory
- Marketplace
- Community
- Platform
---
