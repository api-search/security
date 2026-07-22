---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: captainfresh.in
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: www.captainfresh.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Captain Fresh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Captain Fresh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Captain Fresh
provider_slug: captain-fresh
slug: captain-fresh-domain-security
source_filename: captain-fresh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.captainfresh.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: captainfresh.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captain-fresh/refs/heads/main/security/captain-fresh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Seafood
- Supply Chain
- Marketplace
- B2B
- Food
- Logistics
- India
---
