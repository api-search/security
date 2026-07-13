---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bakerhughes.com
  spf: true
hosts:
- cert_expires: Aug 30 00:25:01 2026 GMT
  host: www.bakerhughes.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baker Hughes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baker Hughes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Baker Hughes
provider_slug: baker-hughes
slug: baker-hughes-domain-security
source_filename: baker-hughes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bakerhughes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 00:25:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bakerhughes.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baker-hughes/refs/heads/main/security/baker-hughes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy Technology
- Industrial IoT
- Oil And Gas
- Asset Performance Management
- Digital Energy
- Fortune 500
---
