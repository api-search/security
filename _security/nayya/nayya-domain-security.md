---
api_specs:
- filename: nayya-benefits-api-openapi.yml
  format: yaml
  label: Nayya Benefits API
  slug: nayya-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-benefits-api-openapi.yml
- filename: nayya-carriers-api-openapi.yml
  format: yaml
  label: Nayya Carriers API
  slug: nayya-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-carriers-api-openapi.yml
- filename: nayya-connections-api-openapi.yml
  format: yaml
  label: Nayya Connections API
  slug: nayya-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-connections-api-openapi.yml
- filename: nayya-dependents-api-openapi.yml
  format: yaml
  label: Nayya Dependents API
  slug: nayya-dependents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-dependents-api-openapi.yml
- filename: nayya-employees-api-openapi.yml
  format: yaml
  label: Nayya Employees API
  slug: nayya-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-employees-api-openapi.yml
- filename: nayya-employers-api-openapi.yml
  format: yaml
  label: Nayya Employers API
  slug: nayya-employers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-employers-api-openapi.yml
- filename: nayya-enrollments-api-openapi.yml
  format: yaml
  label: Nayya Enrollments API
  slug: nayya-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-enrollments-api-openapi.yml
- filename: nayya-recommendations-api-openapi.yml
  format: yaml
  label: Nayya Recommendations API
  slug: nayya-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-recommendations-api-openapi.yml
- filename: nayya-rule-templates-api-openapi.yml
  format: yaml
  label: Nayya Rule Templates API
  slug: nayya-rule-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-rule-templates-api-openapi.yml
- filename: nayya-snapshots-api-openapi.yml
  format: yaml
  label: Nayya Snapshots API
  slug: nayya-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-snapshots-api-openapi.yml
- filename: nayya-token-api-openapi.yml
  format: yaml
  label: Nayya Token API
  slug: nayya-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-token-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nayya.com
  spf: true
hosts:
- cert_expires: Sep 21 15:23:32 2026 GMT
  host: nayya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nayya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nayya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nayya
provider_slug: nayya
slug: nayya-domain-security
source_filename: nayya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nayya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:23:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nayya.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/security/nayya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Employee Benefits
- Insurance
- Insurtech
- Health
- Decision Support
- HR Tech
- Enrollment
- Recommendations
- Artificial Intelligence
---
