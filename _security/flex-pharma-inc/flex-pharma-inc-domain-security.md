---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flex-pharma.com
  spf: false
hosts:
- cert_expires: Sep  6 21:08:02 2026 GMT
  host: www.flex-pharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flex Pharma Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flex Pharma, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Flex Pharma, Inc.
provider_slug: flex-pharma-inc
slug: flex-pharma-inc-domain-security
source_filename: flex-pharma-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flex-pharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 21:08:02 2026 GMT\n  hsts: false\ndomains:\n- domain: flex-pharma.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flex-pharma-inc/refs/heads/main/security/flex-pharma-inc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Pharmaceuticals
- Biotechnology
- Life Sciences
- E-Commerce
- No API
---
