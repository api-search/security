---
api_specs:
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Bills API
  slug: bills
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Intervals API
  slug: intervals
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Meters API
  slug: meters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bayou.energy
  spf: true
hosts:
- cert_expires: Sep  1 17:21:34 2026 GMT
  host: www.bayou.energy
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 05:18:42 2026 GMT
  host: docs.bayou.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: bayou.energy
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bayou Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bayou Energy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bayou Energy
provider_slug: bayou-energy
slug: bayou-energy-domain-security
source_filename: bayou-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bayou.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:21:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.bayou.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 05:18:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bayou.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bayou.energy\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/security/bayou-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Utility Data
- Energy
- Utility Bills
- Interval Data
- Metering
---
