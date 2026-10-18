---
api_specs:
- filename: datia-instruments-api-openapi.yml
  format: yaml
  label: Datia Instruments API
  slug: datia-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datia/refs/heads/main/openapi/datia-instruments-api-openapi.yml
- filename: datia-portfolios-api-openapi.yml
  format: yaml
  label: Datia Portfolios API
  slug: datia-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datia/refs/heads/main/openapi/datia-portfolios-api-openapi.yml
- filename: datia-reports-api-openapi.yml
  format: yaml
  label: Datia Reports API
  slug: datia-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datia/refs/heads/main/openapi/datia-reports-api-openapi.yml
- filename: datia-sustainable-investments-api-openapi.yml
  format: yaml
  label: Datia Sustainable Investments API
  slug: datia-sustainable-investments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datia/refs/heads/main/openapi/datia-sustainable-investments-api-openapi.yml
- filename: datia-taxonomy-api-openapi.yml
  format: yaml
  label: Datia Taxonomy API
  slug: datia-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datia/refs/heads/main/openapi/datia-taxonomy-api-openapi.yml
- filename: datia-temperature-score-api-openapi.yml
  format: yaml
  label: Datia Temperature Score API
  slug: datia-temperature-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datia/refs/heads/main/openapi/datia-temperature-score-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: datia.app
  spf: true
hosts:
- cert_expires: Dec  2 19:12:39 2026 GMT
  host: datia.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Datia
provider_slug: datia
slug: datia-domain-security
source_filename: datia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datia.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 19:12:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datia.app\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datia/refs/heads/main/security/datia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sustainable Finance
- ESG
- Data Platform
- Finance
---
