---
api_specs:
- filename: pentaho-openapi-generated.yml
  format: yaml
  label: Pentaho API
  slug: pentaho-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pentaho/openapi/_ae-authored/pentaho-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pentaho.com
  spf: true
hosts:
- cert_expires: Dec 22 21:59:56 2026 GMT
  host: pentaho.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pentaho Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pentaho, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pentaho
provider_slug: pentaho
slug: pentaho-domain-security
source_filename: pentaho-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pentaho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 21:59:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pentaho.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/pentaho/security/pentaho-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Integration
- Business Analytics
- Embedded Analytics
- AI
- Financial Services
- Healthcare
- Manufacturing
- Government
---
