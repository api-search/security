---
api_specs:
- filename: parabol-graphql-subscriptions-asyncapi.yml
  format: yaml
  label: Parabol GraphQL API
  slug: parabol-graphql-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/parabol/refs/heads/main/asyncapi/parabol-graphql-subscriptions-asyncapi.yml
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
  dmarc_policy: quarantine
  dnssec: true
  domain: parabol.co
  spf: true
hosts:
- cert_expires: Aug 27 22:58:27 2026 GMT
  host: www.parabol.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 11:01:54 2026 GMT
  host: action.parabol.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parabol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parabol, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Parabol
provider_slug: parabol
slug: parabol-domain-security
source_filename: parabol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parabol.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 22:58:27 2026 GMT\n  hsts: false\n- host: action.parabol.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 11:01:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: parabol.co\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parabol/refs/heads/main/security/parabol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- Agile
- Retrospectives
- Meetings
- Collaboration
- GraphQL
- Team Productivity
- Open Source
---
