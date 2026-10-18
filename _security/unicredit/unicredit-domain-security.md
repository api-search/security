---
api_specs:
- filename: unicredit-hydrogen-api-openapi.yml
  format: yaml
  label: UniCredit Hydrogen API
  slug: unicredit-hydrogen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unicredit/refs/heads/main/openapi/unicredit-hydrogen-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: unicredit.eu
  spf: true
hosts:
- cert_expires: Jan 28 10:30:57 2027 GMT
  host: www.unicredit.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Unicredit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UniCredit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: UniCredit
provider_slug: unicredit
slug: unicredit-domain-security
source_filename: unicredit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unicredit.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 10:30:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unicredit.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unicredit/refs/heads/main/security/unicredit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Banking
- Financial Services
- Europe
- Corporate Banking
---
