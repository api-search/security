---
api_specs:
- filename: nuix-nuix-core-engine-rest-api-openapi.yml
  format: yaml
  label: Nuix Core Engine REST API
  slug: nuix-core-engine-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-nuix-core-engine-rest-api-openapi.yml
- filename: nuix-nuix-ecc-rest-api-openapi.yml
  format: yaml
  label: Nuix Enterprise Collection Center REST API
  slug: nuix-ecc-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-nuix-ecc-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nuix.com
  spf: true
hosts:
- cert_expires: Sep 26 12:27:50 2026 GMT
  host: developer.nuix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: documentation.nuix.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- host: discover.nuix.com
  https: false
kind: domain-security
layout: security
method: probed
name: Nuix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuix, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nuix
provider_slug: nuix
slug: nuix-domain-security
source_filename: nuix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.nuix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 12:27:50 2026 GMT\n  hsts: false\n- host: documentation.nuix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: discover.nuix.com\n  https: false\ndomains:\n- domain: nuix.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/security/nuix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Forensics
- eDiscovery
- Investigations
- Compliance
- Data Processing
- Legal Technology
- Intelligence
---
