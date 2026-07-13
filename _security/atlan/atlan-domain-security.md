---
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: atlan.com
  spf: true
hosts:
- cert_expires: Oct  4 08:17:17 2026 GMT
  host: atlan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 06:21:26 2026 GMT
  host: docs.atlan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atlan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atlan, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Atlan
provider_slug: atlan
slug: atlan-domain-security
source_filename: atlan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atlan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:17:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.atlan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 06:21:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atlan.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlan/refs/heads/main/security/atlan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Catalog
- Metadata Management
- Data Governance
- Data Lineage
- GraphQL
- REST
- AI
- Analytics
---
