---
api_specs:
- filename: black-duck-black-duck-api-api-openapi.yml
  format: yaml
  label: Black Duck Black Duck API
  slug: black-duck-black-duck-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/black-duck/refs/heads/main/openapi/black-duck-black-duck-api-api-openapi.yml
- filename: black-duck-issues-api-openapi.yml
  format: yaml
  label: Black Duck Issues API
  slug: black-duck-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/black-duck/refs/heads/main/openapi/black-duck-issues-api-openapi.yml
- filename: black-duck-projects-api-openapi.yml
  format: yaml
  label: Black Duck Projects API
  slug: black-duck-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/black-duck/refs/heads/main/openapi/black-duck-projects-api-openapi.yml
- filename: black-duck-search-api-openapi.yml
  format: yaml
  label: Black Duck Search API
  slug: black-duck-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/black-duck/refs/heads/main/openapi/black-duck-search-api-openapi.yml
- filename: black-duck-users-api-openapi.yml
  format: yaml
  label: Black Duck Users API
  slug: black-duck-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/black-duck/refs/heads/main/openapi/black-duck-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issue "globalsign.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blackduck.com
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: www.blackduck.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 14:54:24 2026 GMT
  host: documentation.blackduck.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 23:59:59 2027 GMT
  host: polaris.blackduck.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Black Duck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Black Duck, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Black Duck
provider_slug: black-duck
slug: black-duck-domain-security
source_filename: black-duck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blackduck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.blackduck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 14:54:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: polaris.blackduck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blackduck.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-duck/refs/heads/main/security/black-duck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Application Security
- Software Composition Analysis
- SAST
- DAST
- Open Source Security
- DevSecOps
- Vulnerability Management
---
