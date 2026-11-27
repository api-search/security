---
api_specs:
- filename: isitdns-net-openapi-generated.yml
  format: yaml
  label: isitdns API
  slug: isitdns-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/isitdns-net/openapi/_ae-authored/isitdns-net-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: isitdns.net
  spf: true
hosts:
- cert_expires: Dec 17 14:39:05 2026 GMT
  host: isitdns.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: isitdns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for isitdns, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: isitdns
provider_slug: isitdns-net
slug: isitdns-net-domain-security
source_filename: isitdns-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: isitdns.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 14:39:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: isitdns.net\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/isitdns-net/security/isitdns-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- DNS
- Monitoring
- Free
---
