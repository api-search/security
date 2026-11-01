---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: virtuous.org
  spf: true
hosts:
- cert_expires: Dec 18 03:44:27 2026 GMT
  host: virtuous.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Virtuous Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virtuous, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Virtuous
provider_slug: virtuous
slug: virtuous-domain-security
source_filename: virtuous-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: virtuous.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 03:44:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: virtuous.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/virtuous/security/virtuous-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Nonprofit
- CRM
- Fundraising
- SaaS
---
