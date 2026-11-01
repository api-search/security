---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: skalelabs.com
  spf: true
hosts:
- cert_expires: Dec 28 12:18:50 2026 GMT
  host: skalelabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Skalelabs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SKALE Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SKALE Labs
provider_slug: skalelabs-com
slug: skalelabs-com-domain-security
source_filename: skalelabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skalelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 12:18:50 2026 GMT\n  hsts: null\ndomains:\n- domain: skalelabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/skalelabs-com/security/skalelabs-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Scaling
- Decentralized
- Infrastructure
---
