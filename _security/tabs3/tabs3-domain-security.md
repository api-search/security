---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tabs3.com
  spf: true
hosts:
- cert_expires: Dec 15 16:38:21 2026 GMT
  host: tabs3.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tabs3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tabs3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tabs3
provider_slug: tabs3
slug: tabs3-domain-security
source_filename: tabs3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tabs3.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 16:38:21 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: tabs3.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tabs3/security/tabs3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- SaaS
- LegalTech
- PracticeManagement
- CloudSoftware
---
