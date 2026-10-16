---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cleanboss.co
  spf: true
hosts:
- cert_expires: Dec 28 02:32:01 2026 GMT
  host: www.cleanboss.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cleanboss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CleanBoss, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CleanBoss
provider_slug: cleanboss
slug: cleanboss-domain-security
source_filename: cleanboss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cleanboss.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 02:32:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: cleanboss.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleanboss/refs/heads/main/security/cleanboss-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Products
- Cleaning
- Eco-friendly
- E‑commerce
---
