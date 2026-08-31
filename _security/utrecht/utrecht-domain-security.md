---
api_specs:
- filename: utrecht-admin-api-openapi.yml
  format: yaml
  label: Utrecht University admin API
  slug: utrecht-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-admin-api-openapi.yml
- filename: utrecht-browse-api-openapi.yml
  format: yaml
  label: Utrecht University browse API
  slug: utrecht-browse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-browse-api-openapi.yml
- filename: utrecht-data-access-token-api-openapi.yml
  format: yaml
  label: Utrecht University data_access_token API
  slug: utrecht-data-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-data-access-token-api-openapi.yml
- filename: utrecht-datarequest-api-openapi.yml
  format: yaml
  label: Utrecht University datarequest API
  slug: utrecht-datarequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-datarequest-api-openapi.yml
- filename: utrecht-folder-api-openapi.yml
  format: yaml
  label: Utrecht University folder API
  slug: utrecht-folder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-folder-api-openapi.yml
- filename: utrecht-groups-api-openapi.yml
  format: yaml
  label: Utrecht University groups API
  slug: utrecht-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-groups-api-openapi.yml
- filename: utrecht-meta-api-openapi.yml
  format: yaml
  label: Utrecht University meta API
  slug: utrecht-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-meta-api-openapi.yml
- filename: utrecht-meta-form-api-openapi.yml
  format: yaml
  label: Utrecht University meta_form API
  slug: utrecht-meta-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-meta-form-api-openapi.yml
- filename: utrecht-notifications-api-openapi.yml
  format: yaml
  label: Utrecht University notifications API
  slug: utrecht-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-notifications-api-openapi.yml
- filename: utrecht-provenance-api-openapi.yml
  format: yaml
  label: Utrecht University provenance API
  slug: utrecht-provenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-provenance-api-openapi.yml
- filename: utrecht-publication-troubleshoot-api-openapi.yml
  format: yaml
  label: Utrecht University publication_troubleshoot API
  slug: utrecht-publication-troubleshoot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-publication-troubleshoot-api-openapi.yml
- filename: utrecht-research-api-openapi.yml
  format: yaml
  label: Utrecht University research API
  slug: utrecht-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-research-api-openapi.yml
- filename: utrecht-revisions-api-openapi.yml
  format: yaml
  label: Utrecht University revisions API
  slug: utrecht-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-revisions-api-openapi.yml
- filename: utrecht-schema-api-openapi.yml
  format: yaml
  label: Utrecht University schema API
  slug: utrecht-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-schema-api-openapi.yml
- filename: utrecht-schema-transformation-api-openapi.yml
  format: yaml
  label: Utrecht University schema_transformation API
  slug: utrecht-schema-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-schema-transformation-api-openapi.yml
- filename: utrecht-settings-api-openapi.yml
  format: yaml
  label: Utrecht University settings API
  slug: utrecht-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-settings-api-openapi.yml
- filename: utrecht-stats-api-openapi.yml
  format: yaml
  label: Utrecht University stats API
  slug: utrecht-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-stats-api-openapi.yml
- filename: utrecht-vault-api-openapi.yml
  format: yaml
  label: Utrecht University vault API
  slug: utrecht-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-vault-api-openapi.yml
- filename: utrecht-vault-archive-api-openapi.yml
  format: yaml
  label: Utrecht University vault_archive API
  slug: utrecht-vault-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-vault-archive-api-openapi.yml
- filename: utrecht-vault-deaccession-api-openapi.yml
  format: yaml
  label: Utrecht University vault_deaccession API
  slug: utrecht-vault-deaccession-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-vault-deaccession-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "harica.gr"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "harica.gr"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: uu.nl
  spf: true
hosts:
- cert_expires: Oct  2 19:54:40 2026 GMT
  host: www.uu.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 23:09:49 2026 GMT
  host: dspace.library.uu.nl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 14:03:46 2026 GMT
  host: portal.yoda.uu.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 06:37:54 2026 GMT
  host: i-lab.yoda.uu.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 10:17:41 2027 GMT
  host: login.uu.nl
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 21:35:52 2026 GMT
  host: research-portal.uu.nl
  hsts: true
  hsts_max_age: 2592000
  https: true
  operator: tenant
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Utrecht Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Utrecht University, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Utrecht University
provider_slug: utrecht
slug: utrecht-domain-security
source_filename: utrecht-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts. Re-probed 2026-08-30 after the Yoda OpenAPIs \n  were re-based off the RFC 2606 placeholder host portal.yoda.test onto the verified production hosts \n  portal.yoda.uu.nl and i-lab.yoda.uu.nl.\nhosts:\n- host: www.uu.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:54:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dspace.library.uu.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:09:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.yoda.uu.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 14:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: i-lab.yoda.uu.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 06:37:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: login.uu.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 10:17:41 2027\
  \ GMT\n  hsts: false\n- host: research-portal.uu.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 21:35:52 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  operator: tenant\ndomains:\n- domain: uu.nl\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/security/utrecht-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Netherlands
- Europe
- Research Data
- Research Data Management
- Institutional Repository
- Identity Federation
- OAI-PMH
- Open Access
- Open Science
- Library
- Open-Source
---
