---
api_specs:
- filename: regulatory-openapi.yml
  format: yaml
  label: FINRA Developer Center API
  slug: finra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regulatory/refs/heads/main/openapi/regulatory-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: finra.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: compliance.ai
  spf: true
hosts:
- cert_expires: Sep 15 03:29:21 2026 GMT
  host: developer.finra.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.compliance.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 01:58:28 2026 GMT
  host: regology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regulatory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regulatory, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Regulatory
provider_slug: regulatory
slug: regulatory-domain-security
source_filename: regulatory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.finra.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:29:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.compliance.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\n- host: regology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 01:58:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: finra.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: compliance.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regulatory/refs/heads/main/security/regulatory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Compliance
- Financial Services
- Governance
- Healthcare Regulation
- Regulatory Reporting
- Risk Management
- RegTech
---
