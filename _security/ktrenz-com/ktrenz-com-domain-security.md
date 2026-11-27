---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ktrenz.com
  spf: false
hosts:
- cert_expires: Dec 31 22:37:49 2026 GMT
  host: ktrenz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KTRENZ Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KTRENZ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: KTRENZ
provider_slug: ktrenz-com
slug: ktrenz-com-domain-security
source_filename: ktrenz-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ktrenz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 22:37:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ktrenz.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ktrenz-com/security/ktrenz-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- K-pop
- Data
- Culture
- Music
---
