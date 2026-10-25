---
api_specs:
- filename: ferc-data-api-openapi.yml
  format: yaml
  label: FERC Data API
  slug: ferc-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-data-api-openapi.yml
- filename: ferc-data-assets-api-openapi.yml
  format: yaml
  label: FERC Data Assets API
  slug: ferc-data-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-data-assets-api-openapi.yml
- filename: ferc-details-api-openapi.yml
  format: yaml
  label: FERC Details API
  slug: ferc-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-details-api-openapi.yml
- filename: ferc-dictionary-api-openapi.yml
  format: yaml
  label: FERC Dictionary API
  slug: ferc-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-dictionary-api-openapi.yml
- filename: ferc-filing-api-openapi.yml
  format: yaml
  label: FERC Filing API
  slug: ferc-filing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-filing-api-openapi.yml
- filename: ferc-public-filings-api-openapi.yml
  format: yaml
  label: FERC Public Filings API
  slug: ferc-public-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-public-filings-api-openapi.yml
- filename: ferc-reference-api-openapi.yml
  format: yaml
  label: FERC Reference API
  slug: ferc-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-reference-api-openapi.yml
- filename: ferc-taxonomy-api-openapi.yml
  format: yaml
  label: FERC Taxonomy API
  slug: ferc-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-taxonomy-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "hostmaster@ferc.gov"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ferc.gov
  spf: true
hosts:
- cert_expires: Dec 10 09:48:04 2026 GMT
  host: www.ferc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 14:54:36 2026 GMT
  host: data.ferc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 18:21:04 2026 GMT
  host: api.data.ferc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ferc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FERC, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FERC
provider_slug: ferc
slug: ferc-domain-security
source_filename: ferc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ferc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 09:48:04 2026 GMT\n  hsts: null\n- host: data.ferc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 14:54:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.data.ferc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 18:21:04 2026 GMT\n  hsts: null\ndomains:\n- domain: ferc.gov\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"hostmaster@ferc.gov\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/security/ferc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- United States
- Energy Markets
- Electricity
- Natural Gas
- Grid
- Regulator
- Government
- Open Data
- Wholesale Power Markets
- Hydropower
- Oil Pipelines
---
