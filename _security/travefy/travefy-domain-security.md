---
api_specs:
- filename: travefy-openapi-generated.yml
  format: yaml
  label: Travefy API
  slug: travefy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/travefy/openapi/_ae-authored/travefy-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: travefy.com
  spf: true
hosts:
- cert_expires: Feb 11 12:24:21 2027 GMT
  host: travefy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Travefy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Travefy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Travefy
provider_slug: travefy
slug: travefy-domain-security
source_filename: travefy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: travefy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 12:24:21 2027 GMT\n  hsts: null\ndomains:\n- domain: travefy.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/travefy/security/travefy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Software
- Software-as-a-Service
- Agency
- CRM
---
