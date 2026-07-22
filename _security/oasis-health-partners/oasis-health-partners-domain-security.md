---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oasishealth.com
  spf: true
hosts:
- cert_expires: Sep  1 01:31:43 2026 GMT
  host: oasishealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oasis Health Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oasis Health Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oasis Health Partners
provider_slug: oasis-health-partners
slug: oasis-health-partners-domain-security
source_filename: oasis-health-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oasishealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 01:31:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oasishealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oasis-health-partners/refs/heads/main/security/oasis-health-partners-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Health
- Healthcare
- Digital Health
- Venture Backed
---
