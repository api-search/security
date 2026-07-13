---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:secops@cdata.com"
  - 0 iodef "mailto:webmaster@cdata.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cdata.com
  spf: true
hosts:
- cert_expires: Sep  3 08:28:21 2026 GMT
  host: www.cdata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 02:14:25 2026 GMT
  host: cloud.cdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CData, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CData
provider_slug: cdata
slug: cdata-domain-security
source_filename: cdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 08:28:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.cdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:14:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cdata.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:secops@cdata.com\"\n  - 0 iodef \"mailto:webmaster@cdata.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/security/cdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Data Access
- Data Connectivity
- Databases
- NoSQL
- SQL
---
