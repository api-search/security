---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pearsuite.com
  spf: true
hosts:
- cert_expires: Oct 16 22:36:33 2026 GMT
  host: pearsuite.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pear Suite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pear Suite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pear Suite
provider_slug: pear-suite
slug: pear-suite-domain-security
source_filename: pear-suite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pearsuite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 22:36:33 2026 GMT\n  hsts: false\ndomains:\n- domain: pearsuite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pear-suite/refs/heads/main/security/pear-suite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Care Management
- Community Health Workers
- Care Coordination
- Medicaid
- SaaS
---
