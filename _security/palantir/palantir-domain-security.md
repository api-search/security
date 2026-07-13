---
api_specs:
- filename: palantir-openapi.yml
  format: yaml
  label: Palantir Foundry API
  slug: palantir-foundry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palantir/refs/heads/main/openapi/palantir-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: palantir.com
  spf: true
hosts:
- cert_expires: Mar 25 17:00:14 2027 GMT
  host: www.palantir.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Palantir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Palantir, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Palantir
provider_slug: palantir
slug: palantir-domain-security
source_filename: palantir-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.palantir.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 25 17:00:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: palantir.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palantir/refs/heads/main/security/palantir-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- AI Platform
- Data Analytics
- Enterprise
- Government
---
