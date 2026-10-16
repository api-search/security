---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: concentricusa.com
  spf: true
hosts:
- cert_expires: Dec  7 14:07:37 2026 GMT
  host: www.concentricusa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Concentricinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Concentricinc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Concentricinc
provider_slug: concentricinc
slug: concentricinc-domain-security
source_filename: concentricinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.concentricusa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 14:07:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: concentricusa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concentricinc/refs/heads/main/security/concentricinc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Power
- Infrastructure
- DataCenter
- Industrial
- Sustainability
---
