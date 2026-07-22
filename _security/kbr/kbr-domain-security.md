---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kbr.com
  spf: true
hosts:
- cert_expires: Jul 29 08:47:47 2026 GMT
  host: www.kbr.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kbr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KBR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KBR
provider_slug: kbr
slug: kbr-domain-security
source_filename: kbr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kbr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 08:47:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: kbr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kbr/refs/heads/main/security/kbr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Defense
- Engineering
- Fortune 500
- Government Services
- Science and Technology
---
