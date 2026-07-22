---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kabal.com
  spf: true
hosts:
- cert_expires: Sep 25 08:02:45 2026 GMT
  host: kabal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kabal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kabal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kabal
provider_slug: kabal
slug: kabal-domain-security
source_filename: kabal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kabal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 08:02:45 2026 GMT\n  hsts: null\ndomains:\n- domain: kabal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kabal/refs/heads/main/security/kabal-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Energy
- Oil and Gas
- Logistics
- Supply Chain
- Maritime
- SaaS
- Operations
---
