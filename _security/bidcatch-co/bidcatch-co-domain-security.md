---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bidcatch.co
  spf: true
hosts:
- cert_expires: Dec 22 00:55:00 2026 GMT
  host: bidcatch.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BidCatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BidCatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BidCatch
provider_slug: bidcatch-co
slug: bidcatch-co-domain-security
source_filename: bidcatch-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bidcatch.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 00:55:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bidcatch.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bidcatch-co/security/bidcatch-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Procurement
- Bids
- EmailDigest
---
