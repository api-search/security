---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kariusdx.com
  spf: true
hosts:
- cert_expires: Oct  1 03:06:12 2026 GMT
  host: kariusdx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Karius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karius, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Karius
provider_slug: karius
slug: karius-domain-security
source_filename: karius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kariusdx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:06:12 2026 GMT\n  hsts: null\ndomains:\n- domain: kariusdx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karius/refs/heads/main/security/karius-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Diagnostics
- Genomics
- Infectious Disease
- Healthcare
- Metagenomics
- Laboratory
- Precision Medicine
---
