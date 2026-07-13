---
api_specs:
- filename: walgreens-store-locator-openapi.yml
  format: yaml
  label: Walgreens Store Locator API
  slug: walgreens-store-locator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-store-locator-openapi.yml
- filename: walgreens-prescription-refill-openapi.yml
  format: yaml
  label: Walgreens Prescription Refill API
  slug: walgreens-prescription-refill
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-prescription-refill-openapi.yml
- filename: walgreens-vaccine-scheduling-openapi.yml
  format: yaml
  label: Walgreens Vaccine Scheduling API
  slug: walgreens-vaccine-scheduling
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-vaccine-scheduling-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: walgreens.com
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.walgreens.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: developer.walgreens.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: services.walgreens.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Walgreens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Walgreens, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Walgreens
provider_slug: walgreens
slug: walgreens-domain-security
source_filename: walgreens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.walgreens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n- host: developer.walgreens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: services.walgreens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: walgreens.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/security/walgreens-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pharmacy
- Healthcare
- Retail
- Prescriptions
- Vaccines
- Fortune 100
---
