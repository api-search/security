---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: directtap.ai
  spf: true
hosts:
- cert_expires: Dec 17 02:53:08 2026 GMT
  host: directtap.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Directtap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DirectTap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DirectTap
provider_slug: directtap
slug: directtap-domain-security
source_filename: directtap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: directtap.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 02:53:08 2026 GMT\n  hsts: false\ndomains:\n- domain: directtap.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/directtap/refs/heads/main/security/directtap-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Restaurant
- SaaS
- Marketplace
- Zero-Commission
- Ordering
---
