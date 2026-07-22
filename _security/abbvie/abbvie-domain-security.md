---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: abbvie.com
  spf: true
hosts:
- cert_expires: Sep 19 03:11:51 2026 GMT
  host: www.abbvie.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abbvie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AbbVie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AbbVie
provider_slug: abbvie
slug: abbvie-domain-security
source_filename: abbvie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abbvie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:11:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: abbvie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abbvie/refs/heads/main/security/abbvie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pharmaceuticals
- Biopharmaceuticals
- Healthcare
- Life Sciences
- Drug Discovery
- Fortune 500
---
