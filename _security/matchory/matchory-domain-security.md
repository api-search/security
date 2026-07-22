---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: matchory.com
  spf: true
hosts:
- cert_expires: Sep 18 07:15:42 2026 GMT
  host: matchory.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 26 10:14:07 2026 GMT
  host: discovery.matchory.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matchory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matchory, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Matchory
provider_slug: matchory
slug: matchory-domain-security
source_filename: matchory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: matchory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 07:15:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: discovery.matchory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 26 10:14:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: matchory.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matchory/refs/heads/main/security/matchory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Procurement
- Supplier Discovery
- Sourcing
- Supply Chain
- Data Enrichment
- Entity Resolution
- Market Intelligence
- Risk Management
- MCP
---
