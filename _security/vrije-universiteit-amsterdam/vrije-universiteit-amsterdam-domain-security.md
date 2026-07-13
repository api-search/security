---
api_specs:
- filename: vrije-universiteit-amsterdam-pure-web-service.yaml
  format: yaml
  label: VU Research Portal Pure Web Service (REST)
  slug: pure-web-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vrije-universiteit-amsterdam/refs/heads/main/openapi/vrije-universiteit-amsterdam-pure-web-service.yaml
description: ''
domains:
- caa:
  - 0 issue "harica.gr"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "digicert.com"
  - 0 issuewild "harica.gr"
  - 0 iodef "mailto:socc@vu.nl"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vu.nl
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:knawnet@knaw.nl"
  - 0 issue "harica.gr"
  - 0 issuewild "harica.gr"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dataverse.nl
  spf: true
hosts:
- cert_expires: Dec 11 05:49:13 2026 GMT
  host: vu.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 07:43:54 2026 GMT
  host: research.vu.nl
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 12:19:21 2026 GMT
  host: dataverse.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vrije Universiteit Amsterdam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vrije Universiteit Amsterdam, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Vrije Universiteit Amsterdam
provider_slug: vrije-universiteit-amsterdam
slug: vrije-universiteit-amsterdam-domain-security
source_filename: vrije-universiteit-amsterdam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vu.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 05:49:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: research.vu.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 07:43:54 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: dataverse.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 12:19:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vu.nl\n  dnssec: true\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"harica.gr\"\n  - 0 iodef \"mailto:socc@vu.nl\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dataverse.nl\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:knawnet@knaw.nl\"\n  - 0 issue \"harica.gr\"\
  \n  - 0 issuewild \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vrije-universiteit-amsterdam/refs/heads/main/security/vrije-universiteit-amsterdam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Netherlands
- Research
- Open Data
- Repository
---
