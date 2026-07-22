---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fortive.com
  spf: true
hosts:
- cert_expires: Sep  8 10:37:27 2026 GMT
  host: www.fortive.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fortive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fortive
provider_slug: fortive
slug: fortive-domain-security
source_filename: fortive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fortive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 10:37:27 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: fortive.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortive/refs/heads/main/security/fortive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fortune 500
- Industrial Technology
- Healthcare Technology
- Automation
- Conglomerate
---
