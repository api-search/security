---
api_specs:
- filename: orcid-address-api-openapi.yml
  format: yaml
  label: ORCID Address API
  slug: orcid-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-address-api-openapi.yml
- filename: orcid-educations-api-openapi.yml
  format: yaml
  label: ORCID Educations API
  slug: orcid-educations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-educations-api-openapi.yml
- filename: orcid-email-api-openapi.yml
  format: yaml
  label: ORCID Email API
  slug: orcid-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-email-api-openapi.yml
- filename: orcid-employments-api-openapi.yml
  format: yaml
  label: ORCID Employments API
  slug: orcid-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-employments-api-openapi.yml
- filename: orcid-external-identifiers-api-openapi.yml
  format: yaml
  label: ORCID External Identifiers API
  slug: orcid-external-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-external-identifiers-api-openapi.yml
- filename: orcid-fundings-api-openapi.yml
  format: yaml
  label: ORCID Fundings API
  slug: orcid-fundings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-fundings-api-openapi.yml
- filename: orcid-keywords-api-openapi.yml
  format: yaml
  label: ORCID Keywords API
  slug: orcid-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-keywords-api-openapi.yml
- filename: orcid-other-names-api-openapi.yml
  format: yaml
  label: ORCID Other Names API
  slug: orcid-other-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-other-names-api-openapi.yml
- filename: orcid-peer-reviews-api-openapi.yml
  format: yaml
  label: ORCID Peer Reviews API
  slug: orcid-peer-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-peer-reviews-api-openapi.yml
- filename: orcid-person-api-openapi.yml
  format: yaml
  label: ORCID Person API
  slug: orcid-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-person-api-openapi.yml
- filename: orcid-personal-details-api-openapi.yml
  format: yaml
  label: ORCID Personal Details API
  slug: orcid-personal-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-personal-details-api-openapi.yml
- filename: orcid-record-api-openapi.yml
  format: yaml
  label: ORCID Record API
  slug: orcid-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-record-api-openapi.yml
- filename: orcid-researcher-urls-api-openapi.yml
  format: yaml
  label: ORCID Researcher Urls API
  slug: orcid-researcher-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-researcher-urls-api-openapi.yml
- filename: orcid-summary-api-openapi.yml
  format: yaml
  label: ORCID Summary API
  slug: orcid-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-summary-api-openapi.yml
- filename: orcid-works-api-openapi.yml
  format: yaml
  label: ORCID Works API
  slug: orcid-works-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-works-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orcid.org
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: orcid.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:14:35 2026 GMT
  host: info.orcid.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: pub.orcid.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orcid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ORCID, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ORCID
provider_slug: orcid
slug: orcid-domain-security
source_filename: orcid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orcid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\n- host: info.orcid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:14:35 2026 GMT\n  hsts: false\n- host: pub.orcid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orcid.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/security/orcid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Academic
- Identity
- Researchers
---
