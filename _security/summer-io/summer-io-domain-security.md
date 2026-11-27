---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: summer.io
  spf: true
hosts:
- cert_expires: Jun  6 18:02:19 2027 GMT
  host: summer.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Summer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Summer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Summer
provider_slug: summer-io
slug: summer-io-domain-security
source_filename: summer-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: summer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jun  6 18:02:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: summer.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/summer-io/security/summer-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- SaaS
- Analytics
- Automation
- Campaigns
- Company
---
