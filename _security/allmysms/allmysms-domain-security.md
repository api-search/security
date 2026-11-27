---
api_specs:
- filename: allmysms-openapi-generated.yml
  format: yaml
  label: All My SMS API
  slug: allmysms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmysms/openapi/_ae-authored/allmysms-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: allmysms.com
  spf: true
hosts:
- cert_expires: Feb  8 06:00:35 2027 GMT
  host: allmysms.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: All My SMS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for All My SMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: All My SMS
provider_slug: allmysms
slug: allmysms-domain-security
source_filename: allmysms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: allmysms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 06:00:35 2027 GMT\n  hsts: false\ndomains:\n- domain: allmysms.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/allmysms/security/allmysms-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- SMS
- Marketing
- Communications
---
