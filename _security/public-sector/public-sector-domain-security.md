---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: data.gov
  spf: true
hosts:
- cert_expires: Sep 16 14:20:54 2026 GMT
  host: api.data.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 12:20:39 2026 GMT
  host: www.data.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 19:11:52 2026 GMT
  host: catalog.data.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Public Sector Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Public Sector, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Public Sector
provider_slug: public-sector
slug: public-sector-domain-security
source_filename: public-sector-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.data.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:20:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.data.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:20:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: catalog.data.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 19:11:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: data.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/public-sector/refs/heads/main/security/public-sector-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Public Sector
- Government
- Federal
- State
- Local
- Civic Tech
- Open Data
- Regulations
- Procurement
- Open Government
- Topic
---
