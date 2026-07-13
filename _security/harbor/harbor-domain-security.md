---
api_specs:
- filename: swagger.json
  format: json
  label: Harbor API
  slug: harbor
  spec_type: OpenAPI
  url: https://api.harbor.gg/docs/v1/swagger.json
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: false
  dnssec: false
  domain: harbor.gg
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: www.harbor.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: api.harbor.gg
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Harbor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harbor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Harbor
provider_slug: harbor
slug: harbor-domain-security
source_filename: harbor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.harbor.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: false\n- host: api.harbor.gg\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: harbor.gg\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbor/refs/heads/main/security/harbor-domain-security.yml
summary_line: TLSv1.3
tags:
- Community
- Engagement
- Loyalty
- Superfans
---
