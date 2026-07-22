---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trellis.law
  spf: true
hosts:
- cert_expires: Sep 14 12:30:22 2026 GMT
  host: trellis.law
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trellis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trellis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trellis
provider_slug: trellis
slug: trellis-domain-security
source_filename: trellis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trellis.law\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:30:22 2026 GMT\n  hsts: null\ndomains:\n- domain: trellis.law\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trellis/refs/heads/main/security/trellis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Legal
- Legal Analytics
- Court Data
- Litigation
- Legal Tech
- Judicial Analytics
- Artificial Intelligence
---
