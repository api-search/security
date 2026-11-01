---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: diffci.com
  spf: true
hosts:
- cert_expires: Jan 18 14:57:15 2027 GMT
  host: diffci.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Diffci Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for diffci-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: diffci-com
provider_slug: diffci-com
slug: diffci-com-domain-security
source_filename: diffci-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diffci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 14:57:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: diffci.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/diffci-com/security/diffci-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CI
- TestSelection
- OpenSource
- SaaS
---
