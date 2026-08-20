---
api_specs:
- filename: mindbody-appointment-api-openapi.yml
  format: yaml
  label: Mindbody Appointment API
  slug: mindbody-appointment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-appointment-api-openapi.yml
- filename: mindbody-class-api-openapi.yml
  format: yaml
  label: Mindbody Class API
  slug: mindbody-class-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-class-api-openapi.yml
- filename: mindbody-client-api-openapi.yml
  format: yaml
  label: Mindbody Client API
  slug: mindbody-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-client-api-openapi.yml
- filename: mindbody-cross-site-api-openapi.yml
  format: yaml
  label: Mindbody Cross Site API
  slug: mindbody-cross-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-cross-site-api-openapi.yml
- filename: mindbody-enrollment-api-openapi.yml
  format: yaml
  label: Mindbody Enrollment API
  slug: mindbody-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-enrollment-api-openapi.yml
- filename: mindbody-metrics-api-openapi.yml
  format: yaml
  label: Mindbody Metrics API
  slug: mindbody-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-metrics-api-openapi.yml
- filename: mindbody-payroll-api-openapi.yml
  format: yaml
  label: Mindbody Payroll API
  slug: mindbody-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-payroll-api-openapi.yml
- filename: mindbody-pick-a-spot-api-openapi.yml
  format: yaml
  label: Mindbody Pick A Spot API
  slug: mindbody-pick-a-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-pick-a-spot-api-openapi.yml
- filename: mindbody-sale-api-openapi.yml
  format: yaml
  label: Mindbody Sale API
  slug: mindbody-sale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-sale-api-openapi.yml
- filename: mindbody-site-api-openapi.yml
  format: yaml
  label: Mindbody Site API
  slug: mindbody-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-site-api-openapi.yml
- filename: mindbody-staff-api-openapi.yml
  format: yaml
  label: Mindbody Staff API
  slug: mindbody-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-staff-api-openapi.yml
- filename: mindbody-subscriptions-api-openapi.yml
  format: yaml
  label: Mindbody Subscriptions API
  slug: mindbody-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-subscriptions-api-openapi.yml
- filename: mindbody-user-token-api-openapi.yml
  format: yaml
  label: Mindbody User Token API
  slug: mindbody-user-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-user-token-api-openapi.yml
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
- Point-of-Sale
- Studios
- Salons
- Spas
- Webhook
---
