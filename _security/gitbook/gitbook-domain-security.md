---
api_specs:
- filename: gitbook-gitbook-api-openapi.yml
  format: yaml
  label: GitBook
  slug: gitbook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-gitbook-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: gitbook.com
  spf: true
hosts:
- cert_expires: Sep 19 19:53:29 2026 GMT
  host: www.gitbook.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 19:53:29 2026 GMT
  host: docs.gitbook.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 19:53:29 2026 GMT
  host: api.gitbook.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gitbook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitBook, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: GitBook
provider_slug: gitbook
slug: gitbook-domain-security
source_filename: gitbook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gitbook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:53:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.gitbook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:53:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gitbook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:53:29 2026 GMT\n  hsts: null\ndomains:\n- domain: gitbook.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/security/gitbook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Content
- Documentation
- Experience
- Integrations
- Platform
- SDKs
---
