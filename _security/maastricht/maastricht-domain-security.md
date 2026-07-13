---
api_specs:
- filename: maastricht-dataversenl.yaml
  format: yaml
  label: DataverseNL Research Data API (Maastricht collection)
  slug: dataversenl
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maastricht/refs/heads/main/openapi/maastricht-dataversenl.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: maastrichtuniversity.nl
  spf: true
- caa:
  - 0 issuewild "harica.gr"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:knawnet@knaw.nl"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dataverse.nl
  spf: true
hosts:
- cert_expires: Aug  6 13:46:37 2026 GMT
  host: www.maastrichtuniversity.nl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 12:59:26 2026 GMT
  host: cris.maastrichtuniversity.nl
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
name: Maastricht Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maastricht University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Maastricht University
provider_slug: maastricht
slug: maastricht-domain-security
source_filename: maastricht-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.maastrichtuniversity.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 13:46:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cris.maastrichtuniversity.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:59:26 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: dataverse.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 12:19:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maastrichtuniversity.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dataverse.nl\n  dnssec: true\n  caa:\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:knawnet@knaw.nl\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maastricht/refs/heads/main/security/maastricht-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Netherlands
- Europe
---
