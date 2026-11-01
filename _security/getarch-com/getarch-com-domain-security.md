---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getarch.com
  spf: true
hosts:
- cert_expires: Dec 23 04:23:54 2026 GMT
  host: www.getarch.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getarch Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arch
provider_slug: getarch-com
slug: getarch-com-domain-security
source_filename: getarch-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getarch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 04:23:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: getarch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getarch-com/security/getarch-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Marketing
- Home Services
- ServiceTitan
---
