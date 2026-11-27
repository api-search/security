---
api_specs:
- filename: lots-directory-lotsdirectory-api-openapi.yml
  format: yaml
  label: LotsDirectory Lotsdirectory API
  slug: lots-directory-lotsdirectory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lots-directory/openapi/lots-directory-lotsdirectory-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lots.directory
  spf: false
hosts:
- cert_expires: Jan  2 11:57:28 2027 GMT
  host: lots.directory
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 11:57:28 2027 GMT
  host: api.lots.directory
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: LotsDirectory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LotsDirectory, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: LotsDirectory
provider_slug: lots-directory
slug: lots-directory-domain-security
source_filename: lots-directory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lots.directory\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 11:57:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lots.directory\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 11:57:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lots.directory\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lots-directory/security/lots-directory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Directories
- Product Launch
- SEO
- Software-as-a-Service
- Launches
---
