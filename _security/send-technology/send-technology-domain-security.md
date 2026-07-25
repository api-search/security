---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: send.technology
  spf: true
hosts:
- cert_expires: Sep  5 14:53:35 2026 GMT
  host: send.technology
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Send Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Send Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Send Technology
provider_slug: send-technology
slug: send-technology-domain-security
source_filename: send-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: send.technology\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 14:53:35 2026 GMT\n  hsts: false\ndomains:\n- domain: send.technology\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/send-technology/refs/heads/main/security/send-technology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- United Kingdom
- Insurtech
- Underwriting
- London Market
- Lloyd's of London
- Specialty Insurance
- Commercial Insurance
- Reinsurance
- Delegated Authority
- MGA
- Policy Administration
- ACORD
- Partner Gated
---
