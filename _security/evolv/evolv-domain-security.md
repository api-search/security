---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Evolv Participant API
  slug: evolv-participant-api
  spec_type: Postman
  url: https://developers.evolv.ai/
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: evolv.ai
  spf: true
hosts:
- cert_expires: Sep 13 20:30:47 2026 GMT
  host: www.evolv.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 02:10:46 2026 GMT
  host: developers.evolv.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: participants.evolv.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evolv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evolv, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Evolv
provider_slug: evolv
slug: evolv-domain-security
source_filename: evolv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evolv.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 20:30:47 2026 GMT\n  hsts: null\n- host: developers.evolv.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:10:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: participants.evolv.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: evolv.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolv/refs/heads/main/security/evolv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Experimentation
- Optimization
- Personalization
- A/B Testing
- Machine Learning
- Conversion Rate Optimization
- Experience Optimization
- Analytics
- Company
---
