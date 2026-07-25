---
api_specs:
- filename: stack-overflow-answers-api-openapi.yml
  format: yaml
  label: Stack Overflow Answers API
  slug: stack-overflow-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-answers-api-openapi.yml
- filename: stack-overflow-articles-api-openapi.yml
  format: yaml
  label: Stack Overflow Articles API
  slug: stack-overflow-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-articles-api-openapi.yml
- filename: stack-overflow-badges-api-openapi.yml
  format: yaml
  label: Stack Overflow Badges API
  slug: stack-overflow-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-badges-api-openapi.yml
- filename: stack-overflow-comments-api-openapi.yml
  format: yaml
  label: Stack Overflow Comments API
  slug: stack-overflow-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-comments-api-openapi.yml
- filename: stack-overflow-questions-api-openapi.yml
  format: yaml
  label: Stack Overflow Questions API
  slug: stack-overflow-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-questions-api-openapi.yml
- filename: stack-overflow-search-api-openapi.yml
  format: yaml
  label: Stack Overflow Search API
  slug: stack-overflow-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-search-api-openapi.yml
- filename: stack-overflow-smes-api-openapi.yml
  format: yaml
  label: Stack Overflow SMEs API
  slug: stack-overflow-smes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-smes-api-openapi.yml
- filename: stack-overflow-tags-api-openapi.yml
  format: yaml
  label: Stack Overflow Tags API
  slug: stack-overflow-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-tags-api-openapi.yml
- filename: stack-overflow-user-groups-api-openapi.yml
  format: yaml
  label: Stack Overflow User Groups API
  slug: stack-overflow-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-user-groups-api-openapi.yml
- filename: stack-overflow-users-api-openapi.yml
  format: yaml
  label: Stack Overflow Users API
  slug: stack-overflow-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 128 iodef "mailto:sysadmin-team@stackoverflow.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stackoverflow.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 128 iodef "mailto:sysadmin-team@stackoverflow.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stackexchange.com
  spf: true
hosts:
- cert_expires: Sep 15 13:00:40 2026 GMT
  host: stackoverflow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 22:33:35 2026 GMT
  host: api.stackexchange.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 09:32:11 2026 GMT
  host: api.stackoverflowteams.com
  hsts: true
  hsts_max_age: 10368000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stack Overflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stack Overflow, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stack Overflow
provider_slug: stack-overflow
slug: stack-overflow-domain-security
source_filename: stack-overflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stackoverflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 13:00:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stackexchange.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 22:33:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stackoverflowteams.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 09:32:11 2026 GMT\n  hsts: true\n  hsts_max_age: 10368000\ndomains:\n- domain: stackoverflow.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 128 iodef \"mailto:sysadmin-team@stackoverflow.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: stackexchange.com\n \
  \ dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 128 iodef \"mailto:sysadmin-team@stackoverflow.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/security/stack-overflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Answers
- Code
- Developer Community
- Developer Tools
- Knowledge Base
- Programming
- Q&A
- Questions
- Stack Overflow
---
