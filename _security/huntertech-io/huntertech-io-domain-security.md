---
api_specs:
- filename: huntertech-io-openapi-generated.yml
  format: yaml
  label: Huntertech API
  slug: huntertech-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/huntertech-io/openapi/_ae-authored/huntertech-io-openapi-generated.yml
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
  dmarc_policy: reject
  dnssec: true
  domain: huntertech.io
  spf: true
hosts:
- cert_expires: Feb  3 08:51:16 2027 GMT
  host: huntertech.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Huntertech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huntertech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Huntertech
provider_slug: huntertech-io
slug: huntertech-io-domain-security
source_filename: huntertech-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: huntertech.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 08:51:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: huntertech.io\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/huntertech-io/security/huntertech-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- VendorIntelligence
- IT
- Incident Management
- Cloud
---
