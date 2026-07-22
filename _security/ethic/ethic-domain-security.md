---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ethic.com
  spf: true
hosts:
- cert_expires: Sep 24 19:03:09 2026 GMT
  host: ethic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ethic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ethic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ethic
provider_slug: ethic
slug: ethic-domain-security
source_filename: ethic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ethic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 19:03:09 2026 GMT\n  hsts: false\ndomains:\n- domain: ethic.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethic/refs/heads/main/security/ethic-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Investing
- Asset Management
- Wealth Management
- Fintech
- Direct Indexing
- ESG
- Values-Based Investing
- Portfolio Management
---
