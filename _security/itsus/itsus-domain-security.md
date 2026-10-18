---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: itsus.nl
  spf: true
hosts:
- cert_expires: Dec 25 04:04:27 2026 GMT
  host: itsus.nl
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Itsus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for It''s Us, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: It's Us
provider_slug: itsus
slug: itsus-domain-security
source_filename: itsus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itsus.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 04:04:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: itsus.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itsus/refs/heads/main/security/itsus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automation
- Business Solutions
- Integration
- SaaS
- Netherlands
---
