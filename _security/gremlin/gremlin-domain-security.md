---
api_specs:
- filename: gremlin-openapi.yml
  format: yaml
  label: Gremlin API
  slug: gremlin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gremlin/refs/heads/main/openapi/gremlin-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@gremlin.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gremlin.com
  spf: true
hosts:
- cert_expires: Oct  7 15:03:25 2026 GMT
  host: www.gremlin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: api.gremlin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gremlin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gremlin, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gremlin
provider_slug: gremlin
slug: gremlin-domain-security
source_filename: gremlin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gremlin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:03:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gremlin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: gremlin.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@gremlin.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gremlin/refs/heads/main/security/gremlin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chaos Engineering
- Fault Injection
- Infrastructure Testing
- Reliability
- Site Reliability Engineering
---
