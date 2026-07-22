---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: geldata.com
  spf: true
hosts:
- cert_expires: Sep 12 08:27:32 2026 GMT
  host: www.geldata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gel Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gel Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gel Data
provider_slug: gel-data
slug: gel-data-domain-security
source_filename: gel-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geldata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 08:27:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: geldata.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gel-data/refs/heads/main/security/gel-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Open Source
- Database
- PostgreSQL
- Graph Database
- GraphQL
- Authentication
- Artificial Intelligence
- Vector Database
- Developer Tools
---
