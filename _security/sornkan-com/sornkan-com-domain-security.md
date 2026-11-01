---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sornkan.com
  spf: true
hosts:
- cert_expires: Jan 25 12:28:25 2027 GMT
  host: sornkan.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sornkan Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sornkan-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: sornkan-com
provider_slug: sornkan-com
slug: sornkan-com-domain-security
source_filename: sornkan-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sornkan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 12:28:25 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: sornkan.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/sornkan-com/security/sornkan-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
