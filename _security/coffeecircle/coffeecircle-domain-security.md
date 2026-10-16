---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coffeecircle.com
  spf: true
hosts:
- cert_expires: Dec 15 05:30:23 2026 GMT
  host: www.coffeecircle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coffeecircle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coffeecircle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coffeecircle
provider_slug: coffeecircle
slug: coffeecircle-domain-security
source_filename: coffeecircle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coffeecircle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 05:30:23 2026 GMT\n  hsts: false\ndomains:\n- domain: coffeecircle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coffeecircle/refs/heads/main/security/coffeecircle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Coffee
- Retail
- E‑commerce
- Sustainability
- Direct‑Trade
---
