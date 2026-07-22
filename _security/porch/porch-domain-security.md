---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: porch.com
  spf: true
hosts:
- cert_expires: Oct 15 04:55:33 2026 GMT
  host: porch.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Porch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Porch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Porch
provider_slug: porch
slug: porch-domain-security
source_filename: porch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: porch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 04:55:33 2026 GMT\n  hsts: null\ndomains:\n- domain: porch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/porch/refs/heads/main/security/porch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Home Services
- Insurance
- InsurTech
- PropTech
- Home Warranty
- Moving
- Real Estate
---
