---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airlabs.co
  spf: true
hosts:
- cert_expires: Oct  1 16:58:36 2026 GMT
  host: airlabs.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airlabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airlabs
provider_slug: airlabs
slug: airlabs-domain-security
source_filename: airlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airlabs.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 16:58:36 2026 GMT\n  hsts: false\ndomains:\n- domain: airlabs.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/security/airlabs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aviation
- Flights
- Airlines
- Airports
- Flight Tracking
- Flight Status
- Real-time Data
---
