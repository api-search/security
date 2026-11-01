---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bidskim.com
  spf: true
hosts:
- cert_expires: Dec 24 01:02:10 2026 GMT
  host: bidskim.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bidskim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BidSkim, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BidSkim
provider_slug: bidskim
slug: bidskim-domain-security
source_filename: bidskim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bidskim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 01:02:10 2026 GMT\n  hsts: false\ndomains:\n- domain: bidskim.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bidskim/security/bidskim-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- procurement
- public-sector
- tenders
- UK
- construction
- AI
---
