---
api_specs:
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Home Services Estimate API
  slug: taskrabbit-home-services-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Home Services Availability API
  slug: taskrabbit-home-services-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Home Services Booking API
  slug: taskrabbit-home-services-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Home Services Catalog API
  slug: taskrabbit-home-services-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Delivery API (Dolly)
  slug: taskrabbit-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: taskrabbit.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dolly.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.taskrabbit.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:09:39 2026 GMT
  host: developer.taskrabbit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 00:43:34 2026 GMT
  host: papi.dolly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taskrabbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TaskRabbit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TaskRabbit
provider_slug: taskrabbit
slug: taskrabbit-domain-security
source_filename: taskrabbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.taskrabbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.taskrabbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:09:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: papi.dolly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 00:43:34 2026 GMT\n  hsts: null\ndomains:\n- domain: taskrabbit.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dolly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/security/taskrabbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gig Economy
- Handyman
- Home Services
- Marketplace
- Delivery
- Moving
- Partner API
- IKEA
---
