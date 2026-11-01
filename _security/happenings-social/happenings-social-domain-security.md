---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: happenings.social
  spf: true
hosts:
- cert_expires: Jan 26 15:24:43 2027 GMT
  host: happenings.social
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Happenings Social Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for happenings-social, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: happenings-social
provider_slug: happenings-social
slug: happenings-social-domain-security
source_filename: happenings-social-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: happenings.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 15:24:43 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: happenings.social\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/happenings-social/security/happenings-social-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Social
- Events
- Platform
- Community
---
