---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: enverus.com
  spf: true
hosts:
- cert_expires: Oct  1 11:54:26 2026 GMT
  host: www.enverus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: app.enverus.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: api.enverus.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Drillinginfo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drillinginfo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Drillinginfo
provider_slug: drillinginfo
slug: drillinginfo-domain-security
source_filename: drillinginfo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enverus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:54:26 2026 GMT\n  hsts: false\n- host: app.enverus.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\n- host: api.enverus.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: enverus.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drillinginfo/refs/heads/main/security/drillinginfo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Oil and Gas
- Data
- Analytics
- Geospatial
- Developer API
- Well Data
- Production Data
- Energy Intelligence
---
