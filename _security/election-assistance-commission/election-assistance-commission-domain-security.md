---
api_specs:
- filename: election-assistance-commission-block-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Block API
  slug: election-assistance-commission-block-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-block-api-openapi.yml
- filename: election-assistance-commission-block-content-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Block Content API
  slug: election-assistance-commission-block-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-block-content-api-openapi.yml
- filename: election-assistance-commission-contact-form-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Contact Form API
  slug: election-assistance-commission-contact-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-contact-form-api-openapi.yml
- filename: election-assistance-commission-date-format-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Date Format API
  slug: election-assistance-commission-date-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-date-format-api-openapi.yml
- filename: election-assistance-commission-file-api-openapi.yml
  format: yaml
  label: Election Assistance Commission File API
  slug: election-assistance-commission-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-file-api-openapi.yml
- filename: election-assistance-commission-media-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Media API
  slug: election-assistance-commission-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-media-api-openapi.yml
- filename: election-assistance-commission-media-type-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Media Type API
  slug: election-assistance-commission-media-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-media-type-api-openapi.yml
- filename: election-assistance-commission-menu-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Menu API
  slug: election-assistance-commission-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-menu-api-openapi.yml
- filename: election-assistance-commission-node-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Node API
  slug: election-assistance-commission-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-node-api-openapi.yml
- filename: election-assistance-commission-node-type-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Node Type API
  slug: election-assistance-commission-node-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-node-type-api-openapi.yml
- filename: election-assistance-commission-paragraph-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Paragraph API
  slug: election-assistance-commission-paragraph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-paragraph-api-openapi.yml
- filename: election-assistance-commission-paragraphs-type-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Paragraphs Type API
  slug: election-assistance-commission-paragraphs-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-paragraphs-type-api-openapi.yml
- filename: election-assistance-commission-search-page-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Search Page API
  slug: election-assistance-commission-search-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-search-page-api-openapi.yml
- filename: election-assistance-commission-taxonomy-term-api-openapi.yml
  format: yaml
  label: Election Assistance Commission Taxonomy Term API
  slug: election-assistance-commission-taxonomy-term-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-taxonomy-term-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eac.gov
  spf: true
hosts:
- cert_expires: Nov  6 21:17:45 2026 GMT
  host: www.eac.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Election Assistance Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Election Assistance Commission, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Election Assistance Commission
provider_slug: election-assistance-commission
slug: election-assistance-commission-domain-security
source_filename: election-assistance-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eac.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 21:17:45 2026 GMT\n  hsts: false\ndomains:\n- domain: eac.gov\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/security/election-assistance-commission-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Elections
- Voting
- Open Data
- Voting Systems
- Certification
- Government Data
- JSON:API
- Public Records
---
