---
api_specs:
- filename: llms.txt
  format: yaml
  label: Oyster HR API
  slug: oyster-hr-api
  spec_type: OpenAPI
  url: https://docs.oysterhr.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: oysterhr.com
  spf: true
hosts:
- cert_expires: Sep 19 15:05:43 2026 GMT
  host: www.oysterhr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 18:56:27 2026 GMT
  host: api.oysterhr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oyster Hr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oyster HR, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Oyster HR
provider_slug: oyster-hr
slug: oyster-hr-domain-security
source_filename: oyster-hr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oysterhr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:05:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.oysterhr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 18:56:27 2026 GMT\n  hsts: null\ndomains:\n- domain: oysterhr.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oyster-hr/refs/heads/main/security/oyster-hr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- HR
- Global Employment
- Payroll
- Employer of Record
- EOR
- Contractors
- Compliance
- Remote Work
---
