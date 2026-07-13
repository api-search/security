---
api_specs:
- filename: env0-openapi.yml
  format: yaml
  label: Env0
  slug: env0
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: env0.com
  spf: true
hosts:
- cert_expires: Aug 17 10:58:24 2026 GMT
  host: www.env0.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: api.env0.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Env0 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Env0, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Env0
provider_slug: env0
slug: env0-domain-security
source_filename: env0-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.env0.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 10:58:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.env0.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: env0.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/security/env0-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- FinOps
- Infrastructure as Code
- DevOps
- Cloud
---
