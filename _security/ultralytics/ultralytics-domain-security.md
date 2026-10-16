---
api_specs:
- filename: ultralytics-openapi-generated.yml
  format: yaml
  label: Ultralytics API
  slug: ultralytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ultralytics/refs/heads/main/openapi/_ae-authored/ultralytics-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@ultralytics.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ultralytics.com
  spf: true
hosts:
- cert_expires: Dec 23 05:10:01 2026 GMT
  host: www.ultralytics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ultralytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ultralytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ultralytics
provider_slug: ultralytics
slug: ultralytics-domain-security
source_filename: ultralytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ultralytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 05:10:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ultralytics.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@ultralytics.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ultralytics/refs/heads/main/security/ultralytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Computer Vision
- AI
- Machine Learning
- Open Source
- SaaS
---
