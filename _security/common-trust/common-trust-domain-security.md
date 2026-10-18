---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: common-trust.com
  spf: true
hosts:
- cert_expires: Dec 24 20:32:06 2026 GMT
  host: www.common-trust.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Common Trust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Common Trust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Common Trust
provider_slug: common-trust
slug: common-trust-domain-security
source_filename: common-trust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.common-trust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 20:32:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: common-trust.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/common-trust/refs/heads/main/security/common-trust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Employee Ownership
- Trust
- EOT
- Advisory
---
