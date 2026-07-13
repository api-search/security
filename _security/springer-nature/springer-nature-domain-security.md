---
api_specs:
- filename: springer-nature-meta-openapi.yml
  format: yaml
  label: Springer Nature Meta API
  slug: springer-nature-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/springer-nature/refs/heads/main/openapi/springer-nature-meta-openapi.yml
- filename: springer-nature-openaccess-openapi.yml
  format: yaml
  label: Springer Nature Open Access API
  slug: springer-nature-openaccess-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/springer-nature/refs/heads/main/openapi/springer-nature-openaccess-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: springernature.com
  spf: true
hosts:
- cert_expires: Aug 18 11:12:04 2026 GMT
  host: dev.springernature.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 11:12:04 2026 GMT
  host: www.springernature.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 07:05:25 2026 GMT
  host: api.springernature.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Springer Nature Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Springer Nature, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Springer Nature
provider_slug: springer-nature
slug: springer-nature-domain-security
source_filename: springer-nature-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.springernature.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 11:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.springernature.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 11:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.springernature.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:05:25 2026 GMT\n  hsts: null\ndomains:\n- domain: springernature.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/springer-nature/refs/heads/main/security/springer-nature-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Academic Publishing
- Open Access
- Research
- Scholarly Content
- Scientific Publishing
---
