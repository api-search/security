---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acornreply.com
  spf: true
hosts:
- cert_expires: Jan 23 08:41:09 2027 GMT
  host: acornreply.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acornreply Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AcornReply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AcornReply
provider_slug: acornreply-com
slug: acornreply-com-domain-security
source_filename: acornreply-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acornreply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 08:41:09 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: acornreply.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/acornreply-com/security/acornreply-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Support
- Software-as-a-Service
- Small Teams
- Artificial Intelligence
- Customer Service
---
