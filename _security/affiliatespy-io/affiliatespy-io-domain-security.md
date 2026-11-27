---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: affiliatespy.io
  spf: false
hosts:
- cert_expires: Dec  8 21:02:28 2026 GMT
  host: affiliatespy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AffiliateSpy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AffiliateSpy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AffiliateSpy
provider_slug: affiliatespy-io
slug: affiliatespy-io-domain-security
source_filename: affiliatespy-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: affiliatespy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 21:02:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: affiliatespy.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/affiliatespy-io/security/affiliatespy-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Affiliate Marketing
- Intelligence
- Artificial Intelligence
- Software-as-a-Service
---
