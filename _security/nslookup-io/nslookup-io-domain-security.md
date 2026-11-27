---
api_specs:
- filename: nslookup-io-dns-api-openapi.yml
  format: yaml
  label: NSLookup.io DNS API
  slug: nslookup-io-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nslookup-io/openapi/nslookup-io-dns-api-openapi.yml
- filename: nslookup-io-geo-api-openapi.yml
  format: yaml
  label: NSLookup.io GEO API
  slug: nslookup-io-geo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nslookup-io/openapi/nslookup-io-geo-api-openapi.yml
- filename: nslookup-io-monitoring-api-openapi.yml
  format: yaml
  label: NSLookup.io Monitoring API
  slug: nslookup-io-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nslookup-io/openapi/nslookup-io-monitoring-api-openapi.yml
- filename: nslookup-io-security-api-openapi.yml
  format: yaml
  label: NSLookup.io Security API
  slug: nslookup-io-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nslookup-io/openapi/nslookup-io-security-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "ops@easydmarc.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nslookup.io
  spf: true
hosts:
- cert_expires: Feb  4 14:10:23 2027 GMT
  host: nslookup.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NSLookup.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NSLookup.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NSLookup.io
provider_slug: nslookup-io
slug: nslookup-io-domain-security
source_filename: nslookup-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nslookup.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 14:10:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nslookup.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"ops@easydmarc.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nslookup-io/security/nslookup-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DNS
- Network Tools
- Monitoring
- Developers
---
