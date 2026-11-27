---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eleyed.com
  spf: true
hosts:
- cert_expires: Dec 29 17:33:01 2026 GMT
  host: eleyed.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: eleyed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eleyed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: eleyed
provider_slug: eleyed-com
slug: eleyed-com-domain-security
source_filename: eleyed-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eleyed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 17:33:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eleyed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/eleyed-com/security/eleyed-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Privacy
- Document-Redaction
- Artificial Intelligence
- Data Protection
- Software-as-a-Service
- Company
---
