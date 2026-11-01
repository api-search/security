---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: trussle.com
  spf: true
hosts:
- cert_expires: Dec  5 06:51:04 2026 GMT
  host: trussle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trussle Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trussle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Trussle
provider_slug: trussle-com
slug: trussle-com-domain-security
source_filename: trussle-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trussle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 06:51:04 2026 GMT\n  hsts: false\ndomains:\n- domain: trussle.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/trussle-com/security/trussle-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Mortgage
- FinTech
- UK
- Broker
- Digital
---
