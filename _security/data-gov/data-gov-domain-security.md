---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: data.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ckan.org
  spf: true
hosts:
- cert_expires: Oct  3 14:20:38 2026 GMT
  host: data.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 10:44:02 2026 GMT
  host: docs.ckan.org
  hsts: false
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
name: Data Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data.gov, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Data.gov
provider_slug: data-gov
slug: data-gov-domain-security
source_filename: data-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:20:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ckan.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 10:44:02 2026 GMT\n  hsts: false\n- host: catalog.data.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 19:11:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: data.gov\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ckan.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-gov/refs/heads/main/security/data-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Open Data
- Catalog
- CKAN
- Datasets
- Federal
- GSA
- Open Government
---
