---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: irs.gov
  spf: true
- caa: []
  dmarc: true
  dnssec: false
  domain: taxjar.com
  spf: true
hosts:
- cert_expires: Aug 24 05:55:53 2026 GMT
  host: www.irs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 12:33:10 2026 GMT
  host: la1.www4.irs.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 23:15:29 2026 GMT
  host: developers.taxjar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tax Reporting Templates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tax Reporting Templates, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tax Reporting Templates
provider_slug: tax-reporting-templates
slug: tax-reporting-templates-domain-security
source_filename: tax-reporting-templates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.irs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 05:55:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: la1.www4.irs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 12:33:10 2026 GMT\n  hsts: null\n- host: developers.taxjar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:15:29 2026 GMT\n  hsts: false\ndomains:\n- domain: irs.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: taxjar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tax-reporting-templates/refs/heads/main/security/tax-reporting-templates-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Compliance
- Documentation
- Finance
- Reporting
- Tax
- Templates
---
