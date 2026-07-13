---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trinet.com
  spf: true
hosts:
- cert_expires: Sep 19 15:53:52 2026 GMT
  host: www.trinet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: apidocs.trinet.com
  https: false
- cert_expires: Jul 20 23:59:59 2026 GMT
  host: api.trinet.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Trinet Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TriNet Group, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TriNet Group
provider_slug: trinet-group
slug: trinet-group-domain-security
source_filename: trinet-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trinet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:53:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.trinet.com\n  https: false\n- host: api.trinet.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trinet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trinet-group/refs/heads/main/security/trinet-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Benefits
- Compliance
- Human Resources
- Payroll
- Professional Employer Organization
- Risk Management
- Fortune 1000
---
