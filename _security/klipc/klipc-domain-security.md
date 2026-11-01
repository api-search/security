---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: klipc.com
  spf: true
hosts:
- cert_expires: Dec 24 13:08:40 2026 GMT
  host: klipc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Klipc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KlipC Cloud Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KlipC Cloud Systems
provider_slug: klipc
slug: klipc-domain-security
source_filename: klipc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: klipc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 13:08:40 2026 GMT\n  hsts: false\ndomains:\n- domain: klipc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/klipc/security/klipc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
