---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thisisalice.com
  spf: true
hosts:
- cert_expires: Jan 19 14:14:31 2027 GMT
  host: thisisalice.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thisisalice Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alice
provider_slug: thisisalice-com
slug: thisisalice-com-domain-security
source_filename: thisisalice-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thisisalice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 14:14:31 2027 GMT\n  hsts: false\ndomains:\n- domain: thisisalice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/thisisalice-com/security/thisisalice-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- FinTech
- Benefits
- Payroll
- EmployeeExperience
---
