---
api_specs:
- filename: mindbody-public-api-v6-openapi-original.yml
  format: yaml
  label: Mindbody Public API v6
  slug: public-api-v6
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-public-api-v6-openapi-original.yml
- filename: mindbody-webhooks-api-openapi-original.yml
  format: yaml
  label: Mindbody Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-webhooks-api-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mindbodyonline.com
  spf: true
hosts:
- cert_expires: Sep  6 20:16:44 2026 GMT
  host: www.mindbodyonline.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 19:01:45 2026 GMT
  host: developers.mindbodyonline.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 19:01:45 2026 GMT
  host: api.mindbodyonline.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mindbody Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mindbody, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mindbody
provider_slug: mindbody
slug: mindbody-domain-security
source_filename: mindbody-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mindbodyonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 20:16:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developers.mindbodyonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:01:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.mindbodyonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:01:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mindbodyonline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/security/mindbody-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Wellness
- Beauty
- Scheduling
- Booking
- Point of Sale
- Studios
- Salons
- Spas
- Webhooks
---
