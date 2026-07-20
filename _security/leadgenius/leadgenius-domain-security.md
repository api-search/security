---
api_specs:
- filename: leadgenius-enrichment-api-openapi.yml
  format: yaml
  label: LeadGenius Enrichment API
  slug: leadgenius-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadgenius/refs/heads/main/openapi/leadgenius-enrichment-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leadgenius.com
  spf: true
hosts:
- cert_expires: Oct 14 22:51:01 2026 GMT
  host: leadgenius.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 11:34:31 2026 GMT
  host: docs.leadgenius.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leadgenius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeadGenius, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LeadGenius
provider_slug: leadgenius
slug: leadgenius-domain-security
source_filename: leadgenius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leadgenius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:51:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.leadgenius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 11:34:31 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: leadgenius.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadgenius/refs/heads/main/security/leadgenius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Enrichment
- Lead Generation
- Sales
- Marketing
- B2B Data
- Contact Data
- Firmographics
- Go To Market
- Account Based Marketing
---
