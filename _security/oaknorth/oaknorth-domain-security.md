---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oaknorth.co.uk
  spf: true
hosts:
- cert_expires: Sep 15 16:34:18 2026 GMT
  host: oaknorth.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oaknorth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OakNorth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OakNorth
provider_slug: oaknorth
slug: oaknorth-domain-security
source_filename: oaknorth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oaknorth.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:34:18 2026 GMT\n  hsts: false\ndomains:\n- domain: oaknorth.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oaknorth/refs/heads/main/security/oaknorth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Banking
- Lending
- Commercial Real Estate
- Business Banking
- Savings
- SME Finance
---
