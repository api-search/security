---
api_specs:
- filename: docs
  format: yaml
  label: G-P Authentication API
  slug: g-p-authentication-api
  spec_type: OpenAPI
  url: https://developer.g-p.com/apis/authentication-1/docs
- filename: docs
  format: yaml
  label: G-P EOR API
  slug: g-p-eor-api
  spec_type: OpenAPI
  url: https://developer.g-p.com/apis/eor/docs
- filename: docs
  format: yaml
  label: G-P Contractor API
  slug: g-p-contractor-api
  spec_type: OpenAPI
  url: https://developer.g-p.com/apis/contractor/docs
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: globalization-partners.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: g-p.com
  spf: true
hosts:
- cert_expires: Aug 12 17:14:39 2026 GMT
  host: www.globalization-partners.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 22:13:33 2026 GMT
  host: developer.g-p.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: api.g-p.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: G P Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for G-P, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: G-P
provider_slug: g-p
slug: g-p-domain-security
source_filename: g-p-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.globalization-partners.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 17:14:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.g-p.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 22:13:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.g-p.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: globalization-partners.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: g-p.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/g-p/refs/heads/main/security/g-p-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Global Employment
- Employer of Record
- EOR
- Payroll
- HR
- Compliance
- Contractors
- International Hiring
---
