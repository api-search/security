---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: axs.com
  spf: true
hosts:
- cert_expires: Dec 14 21:17:20 2026 GMT
  host: www.axs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AXS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AXS
provider_slug: axs
slug: axs-domain-security
source_filename: axs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 21:17:20 2026 GMT\n  hsts: null\ndomains:\n- domain: axs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axs/refs/heads/main/security/axs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
