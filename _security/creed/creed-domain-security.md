---
api_specs:
- filename: creed-openapi-original.json
  format: json
  label: Creed API
  slug: creed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creed/refs/heads/main/openapi/creed-openapi-original.json
description: ''
domains:
- caa:
  - creed-lander-neldq.ondigitalocean.app.
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: usecreed.com
  spf: true
hosts:
- cert_expires: Sep 28 05:27:06 2026 GMT
  host: usecreed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 15:03:23 2026 GMT
  host: api.usecreed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Creed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creed, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Creed
provider_slug: creed
slug: creed-domain-security
source_filename: creed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usecreed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:27:06 2026 GMT\n  hsts: false\n- host: api.usecreed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 15:03:23 2026 GMT\n  hsts: null\ndomains:\n- domain: usecreed.com\n  dnssec: true\n  caa:\n  - creed-lander-neldq.ondigitalocean.app.\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creed/refs/heads/main/security/creed-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Faith
- Religion
- Christianity
- Bible
- Prayer
- Artificial Intelligence
- Chatbot
- Consumer
- Community
---
