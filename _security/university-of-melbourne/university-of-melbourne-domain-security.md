---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unimelb.edu.au
  spf: true
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arcgis.com
  spf: true
hosts:
- cert_expires: Oct  6 20:47:56 2026 GMT
  host: www.unimelb.edu.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 00:18:39 2026 GMT
  host: minerva-access.unimelb.edu.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: spatialdata-uom.opendata.arcgis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Melbourne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Melbourne, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Melbourne
provider_slug: university-of-melbourne
slug: university-of-melbourne-domain-security
source_filename: university-of-melbourne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unimelb.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 20:47:56 2026 GMT\n  hsts: null\n- host: minerva-access.unimelb.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 00:18:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: spatialdata-uom.opendata.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unimelb.edu.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: arcgis.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-melbourne/refs/heads/main/security/university-of-melbourne-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Australia
- Open Data
- Research
- Library
- Repository
---
