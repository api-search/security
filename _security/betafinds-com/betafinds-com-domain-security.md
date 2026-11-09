---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: betafinds.com
  spf: true
hosts:
- cert_expires: Dec 12 05:25:58 2026 GMT
  host: betafinds.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Betafinds Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetaFinds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BetaFinds
provider_slug: betafinds-com
slug: betafinds-com-domain-security
source_filename: betafinds-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betafinds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 05:25:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: betafinds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/betafinds-com/security/betafinds-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Startups
- Platform
- Community
- Discovery
---
