---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: incrediblefi.com
  spf: true
hosts:
- cert_expires: Jan 22 05:00:43 2027 GMT
  host: incrediblefi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IncredibleFi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IncredibleFi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IncredibleFi
provider_slug: incrediblefi-com
slug: incrediblefi-com-domain-security
source_filename: incrediblefi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: incrediblefi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 05:00:43 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: incrediblefi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/incrediblefi-com/security/incrediblefi-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Personal Loans
- Loan Marketplace
- Fintech
- Consumer Lending
---
