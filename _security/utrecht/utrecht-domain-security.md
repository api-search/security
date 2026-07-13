---
api_specs:
- filename: utrecht-yoda-core.yaml
  format: yaml
  label: Yoda Research Data Management Platform
  slug: yoda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-yoda-core.yaml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "harica.gr"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "harica.gr"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: uu.nl
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: yoda.test
  spf: false
hosts:
- cert_expires: Oct  2 19:54:40 2026 GMT
  host: www.uu.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 23:09:49 2026 GMT
  host: dspace.library.uu.nl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: portal.yoda.test
  https: false
kind: domain-security
layout: security
method: probed
name: Utrecht Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Utrecht University, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Utrecht University
provider_slug: utrecht
slug: utrecht-domain-security
source_filename: utrecht-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uu.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:54:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dspace.library.uu.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:09:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.yoda.test\n  https: false\ndomains:\n- domain: uu.nl\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: yoda.test\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/security/utrecht-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Netherlands
- Research Data
- Open Access
- Library
- Open Source
---
