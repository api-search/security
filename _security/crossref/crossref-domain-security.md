---
api_specs:
- filename: crossref-agency-api-openapi.yml
  format: yaml
  label: Crossref Agency API
  slug: crossref-agency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossref/refs/heads/main/openapi/crossref-agency-api-openapi.yml
- filename: crossref-funders-api-openapi.yml
  format: yaml
  label: Crossref Funders API
  slug: crossref-funders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossref/refs/heads/main/openapi/crossref-funders-api-openapi.yml
- filename: crossref-journals-api-openapi.yml
  format: yaml
  label: Crossref Journals API
  slug: crossref-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossref/refs/heads/main/openapi/crossref-journals-api-openapi.yml
- filename: crossref-licenses-api-openapi.yml
  format: yaml
  label: Crossref Licenses API
  slug: crossref-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossref/refs/heads/main/openapi/crossref-licenses-api-openapi.yml
- filename: crossref-members-api-openapi.yml
  format: yaml
  label: Crossref Members API
  slug: crossref-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossref/refs/heads/main/openapi/crossref-members-api-openapi.yml
- filename: crossref-prefixes-api-openapi.yml
  format: yaml
  label: Crossref Prefixes API
  slug: crossref-prefixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossref/refs/heads/main/openapi/crossref-prefixes-api-openapi.yml
- filename: crossref-types-api-openapi.yml
  format: yaml
  label: Crossref Types API
  slug: crossref-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossref/refs/heads/main/openapi/crossref-types-api-openapi.yml
- filename: crossref-works-api-openapi.yml
  format: yaml
  label: Crossref Works API
  slug: crossref-works-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossref/refs/heads/main/openapi/crossref-works-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crossref.org
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.crossref.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: api.crossref.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crossref Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crossref, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crossref
provider_slug: crossref
slug: crossref-domain-security
source_filename: crossref-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crossref.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\n- host: api.crossref.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: crossref.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossref/refs/heads/main/security/crossref-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Citations
- DOI
- Funders
- Identifiers
- Journals
- Licenses
- Members
- Metadata
- Open Access
- ORCID
- Prefixes
- Publishers
- Reference Linking
- ROR
- Scholarly
---
