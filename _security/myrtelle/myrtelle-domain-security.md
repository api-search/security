---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: myrtellegtx.com
  spf: true
hosts:
- cert_expires: Nov  9 05:39:19 2026 GMT
  host: myrtellegtx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Myrtelle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Myrtelle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Myrtelle
provider_slug: myrtelle
slug: myrtelle-domain-security
source_filename: myrtelle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myrtellegtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 05:39:19 2026 GMT\n  hsts: null\ndomains:\n- domain: myrtellegtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myrtelle/refs/heads/main/security/myrtelle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Gene Therapy
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Rare Disease
- Healthcare
---
