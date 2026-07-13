---
description: ''
domains:
- caa:
  - 0 issue "harica.gr"
  - 0 iodef "mailto:admin@ucm.es"
  - 0 issuewild "harica.gr"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ucm.es
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: universidata.es
  spf: false
hosts:
- cert_expires: Dec  4 08:18:56 2026 GMT
  host: www.ucm.es
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 14:58:01 2026 GMT
  host: www.universidata.es
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 20:52:45 2026 GMT
  host: universidatacatalog.azurewebsites.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Complutense University Of Madrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Complutense University of Madrid, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Complutense University of Madrid
provider_slug: complutense-university-of-madrid
slug: complutense-university-of-madrid-domain-security
source_filename: complutense-university-of-madrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucm.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 08:18:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.universidata.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:58:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: universidatacatalog.azurewebsites.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 20:52:45 2026 GMT\n  hsts: null\ndomains:\n- domain: ucm.es\n  dnssec: false\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 iodef \"mailto:admin@ucm.es\"\n  - 0 issuewild \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: universidata.es\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/complutense-university-of-madrid/refs/heads/main/security/complutense-university-of-madrid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Research
- Spain
---
