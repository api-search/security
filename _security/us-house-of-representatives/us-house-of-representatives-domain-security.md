---
api_specs:
- filename: congress-gov-api-openapi.yml
  format: yaml
  label: Congress.gov API
  slug: congress-gov-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-house-of-representatives/refs/heads/main/openapi/congress-gov-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: loc.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: propublica.org
  spf: true
hosts:
- cert_expires: Sep 12 02:51:22 2026 GMT
  host: www.loc.gov
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 18:21:20 2026 GMT
  host: projects.propublica.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 11:20:55 2026 GMT
  host: api.congress.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us House Of Representatives Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US House of Representatives, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: US House of Representatives
provider_slug: us-house-of-representatives
slug: us-house-of-representatives-domain-security
source_filename: us-house-of-representatives-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:51:22 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: projects.propublica.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 18:21:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.congress.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:20:55 2026 GMT\n  hsts: null\ndomains:\n- domain: loc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: propublica.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-house-of-representatives/refs/heads/main/security/us-house-of-representatives-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Legislation
- Congress
- Legislative Data
- Bills
- Members
- Committees
---
