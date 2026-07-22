---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: werevalence.com
  spf: true
hosts:
- cert_expires: Oct 19 16:18:10 2026 GMT
  host: werevalence.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Valence
provider_slug: valence
slug: valence-domain-security
source_filename: valence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: werevalence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 16:18:10 2026 GMT\n  hsts: false\ndomains:\n- domain: werevalence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valence/refs/heads/main/security/valence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mental Health
- Healthcare
- Therapy
- Artificial Intelligence
- Clinical Support
---
