---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aarven.ch
  spf: true
hosts:
- cert_expires: Dec 17 13:32:44 2026 GMT
  host: aarven.ch
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aarven Ch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aarven, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aarven
provider_slug: aarven-ch
slug: aarven-ch-domain-security
source_filename: aarven-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aarven.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 13:32:44 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: aarven.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aarven-ch/security/aarven-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Artificial Intelligence
- Bookkeeping
- Swiss
- Finance
- Automation
---
