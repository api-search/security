---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wecantrack.com
  spf: true
hosts:
- cert_expires: Oct  6 01:26:46 2026 GMT
  host: docs.wecantrack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wecantrack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeCanTrack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WeCanTrack
provider_slug: wecantrack
slug: wecantrack-domain-security
source_filename: wecantrack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.wecantrack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:26:46 2026 GMT\n  hsts: false\ndomains:\n- domain: wecantrack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wecantrack/refs/heads/main/security/wecantrack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Tracking
- Public APIs
---
