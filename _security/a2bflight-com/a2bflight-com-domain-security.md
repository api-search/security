---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: a2bflight.com
  spf: true
hosts:
- cert_expires: Dec 17 02:26:03 2026 GMT
  host: a2bflight.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: a2bflight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for a2bflight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: a2bflight
provider_slug: a2bflight-com
slug: a2bflight-com-domain-security
source_filename: a2bflight-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: a2bflight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 02:26:03 2026 GMT\n  hsts: false\ndomains:\n- domain: a2bflight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/a2bflight-com/security/a2bflight-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Flights
- Search
- Pricing
- Collaboration
---
