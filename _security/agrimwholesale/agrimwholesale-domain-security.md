---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agrim.app
  spf: true
hosts:
- cert_expires: Dec  2 10:08:20 2026 GMT
  host: agrim.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agrimwholesale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agrim Wholesale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agrim Wholesale
provider_slug: agrimwholesale
slug: agrimwholesale-domain-security
source_filename: agrimwholesale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agrim.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 10:08:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agrim.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrimwholesale/refs/heads/main/security/agrimwholesale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- AgriTech
- Wholesale
- B2B
- Marketplace
- E-Commerce
- Supply Chain
- India
---
