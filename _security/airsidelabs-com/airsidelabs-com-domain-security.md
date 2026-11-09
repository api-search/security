---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: airsidelabs.com
  spf: true
hosts:
- cert_expires: Dec 24 11:38:06 2026 GMT
  host: airsidelabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airsidelabs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airside Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Airside Labs
provider_slug: airsidelabs-com
slug: airsidelabs-com-domain-security
source_filename: airsidelabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airsidelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 11:38:06 2026 GMT\n  hsts: false\ndomains:\n- domain: airsidelabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/airsidelabs-com/security/airsidelabs-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Aviation
- Travel
- Infrastructure
- Platform
---
