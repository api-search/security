---
api_specs:
- filename: wappalyzer-v2-public-openapi.yaml
  format: yaml
  label: Wappalyzer Public API
  slug: wappalyzer-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/_original/wappalyzer-v2-public-openapi.yaml
- filename: wappalyzer-metadata-api-openapi.yml
  format: yaml
  label: Wappalyzer Metadata API
  slug: wappalyzer-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/wappalyzer-metadata-api-openapi.yml
- filename: wappalyzer-basics-api-openapi.yml
  format: yaml
  label: Wappalyzer Basics API
  slug: wappalyzer-basics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/wappalyzer-basics-api-openapi.yml
- filename: wappalyzer-lists-api-openapi.yml
  format: yaml
  label: Wappalyzer Lists API
  slug: wappalyzer-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/wappalyzer-lists-api-openapi.yml
- filename: wappalyzer-lookup-api-openapi.yml
  format: yaml
  label: Wappalyzer Lookup API
  slug: wappalyzer-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/wappalyzer-lookup-api-openapi.yml
- filename: wappalyzer-subdomains-api-openapi.yml
  format: yaml
  label: Wappalyzer Subdomains API
  slug: wappalyzer-subdomains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/wappalyzer-subdomains-api-openapi.yml
- filename: wappalyzer-verify-api-openapi.yml
  format: yaml
  label: Wappalyzer Verify API
  slug: wappalyzer-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/wappalyzer-verify-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wappalyzer.com
  spf: true
hosts:
- cert_expires: Nov  9 11:42:59 2026 GMT
  host: www.wappalyzer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 11:42:59 2026 GMT
  host: api.wappalyzer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wappalyzer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wappalyzer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wappalyzer
provider_slug: wappalyzer
slug: wappalyzer-domain-security
source_filename: wappalyzer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wappalyzer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 11:42:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.wappalyzer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 11:42:59 2026 GMT\n  hsts: false\ndomains:\n- domain: wappalyzer.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/security/wappalyzer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Technology Detection
- Technographics
- Website Analysis
- CMS Detection
- Framework Detection
- Lead Enrichment
- Sales Intelligence
- Subdomain Discovery
- Email Verification
- Market Research
---
