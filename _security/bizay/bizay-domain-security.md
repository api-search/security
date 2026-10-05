---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bizay.com
  spf: true
hosts:
- cert_expires: Dec  4 11:10:35 2026 GMT
  host: us.bizay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bizay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bizay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bizay
provider_slug: bizay
slug: bizay-domain-security
source_filename: bizay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: us.bizay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 11:10:35 2026 GMT\n  hsts: null\ndomains:\n- domain: bizay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bizay/refs/heads/main/security/bizay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Print on Demand
- Marketing
- Customization
---
