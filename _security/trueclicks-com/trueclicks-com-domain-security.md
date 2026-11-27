---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: trueclicks.com
  spf: true
hosts:
- cert_expires: Feb  3 17:56:41 2027 GMT
  host: trueclicks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TrueClicks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrueClicks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TrueClicks
provider_slug: trueclicks-com
slug: trueclicks-com-domain-security
source_filename: trueclicks-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trueclicks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 17:56:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trueclicks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/trueclicks-com/security/trueclicks-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- PPC
- Marketing
- Advertising
- SaaS
---
