---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: artificial.io
  spf: true
hosts:
- cert_expires: Sep 21 14:13:50 2026 GMT
  host: artificial.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Artificial Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artificial Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Artificial Labs
provider_slug: artificial-labs
slug: artificial-labs-domain-security
source_filename: artificial-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artificial.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:13:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: artificial.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artificial-labs/refs/heads/main/security/artificial-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Insurtech
- Underwriting
- Reinsurance
- Specialty Insurance
- London Market
- Lloyd's of London
- Broker
- Policy Administration
- ACORD
- Algorithmic Underwriting
---
