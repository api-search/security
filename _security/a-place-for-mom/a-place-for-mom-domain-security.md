---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aplaceformom.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.aplaceformom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: A Place For Mom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A Place for Mom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: A Place for Mom
provider_slug: a-place-for-mom
slug: a-place-for-mom-domain-security
source_filename: a-place-for-mom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aplaceformom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aplaceformom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a-place-for-mom/refs/heads/main/security/a-place-for-mom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Senior Living
- Senior Care
- Referral Marketplace
- Home Care
- Healthcare
- Reviews
- Lead Generation
---
