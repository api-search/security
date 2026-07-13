---
api_specs:
- filename: stack-overflow-openapi.yml
  format: yaml
  label: Stack Overflow API
  slug: stack-overflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-openapi.yml
- filename: stack-overflow-for-teams-openapi.yml
  format: yaml
  label: Stack Overflow for Teams API v3
  slug: stack-overflow-for-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-for-teams-openapi.yml
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
