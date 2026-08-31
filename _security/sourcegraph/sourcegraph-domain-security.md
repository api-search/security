---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sourcegraph.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ampcode.com
  spf: true
hosts:
- cert_expires: Aug 14 02:55:58 2026 GMT
  host: sourcegraph.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 22:11:19 2026 GMT
  host: ampcode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sourcegraph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sourcegraph, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Sourcegraph
provider_slug: sourcegraph
slug: sourcegraph-domain-security
source_filename: sourcegraph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sourcegraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:55:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ampcode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 22:11:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sourcegraph.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ampcode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourcegraph/refs/heads/main/security/sourcegraph-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Code Intelligence
- Code Search
- Cody
- Amp
- AI Coding Agent
- GraphQL
- REST API
- MCP
---
