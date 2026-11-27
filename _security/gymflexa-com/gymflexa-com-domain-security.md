---
api_specs:
- filename: gymflexa-com-api-openapi.json
  format: json
  label: GymFlexa API API
  slug: gymflexa-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gymflexa-com/openapi/_original/gymflexa-com-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gymflexa.com
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: gymflexa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GymFlexa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GymFlexa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GymFlexa
provider_slug: gymflexa-com
slug: gymflexa-com-domain-security
source_filename: gymflexa-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gymflexa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: gymflexa.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gymflexa-com/security/gymflexa-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fitness
- Software-as-a-Service
- Gym Management
- Membership
- Scheduling
---
