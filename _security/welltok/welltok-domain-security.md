---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: welltok.com
  spf: true
hosts:
- cert_expires: Aug 25 07:36:52 2026 GMT
  host: www.welltok.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Welltok Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Welltok, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Welltok
provider_slug: welltok
slug: welltok-domain-security
source_filename: welltok-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.welltok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 07:36:52 2026 GMT\n  hsts: false\ndomains:\n- domain: welltok.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/welltok/refs/heads/main/security/welltok-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- SaaS
- Consumer Engagement
- Consumer Activation
- Health Plans
- Population Health
---
