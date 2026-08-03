---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tidalvision.com
  spf: true
hosts:
- cert_expires: Oct 20 05:45:30 2026 GMT
  host: tidalvision.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tidal Vision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tidal Vision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tidal Vision
provider_slug: tidal-vision
slug: tidal-vision-domain-security
source_filename: tidal-vision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tidalvision.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 05:45:30 2026 GMT\n  hsts: false\ndomains:\n- domain: tidalvision.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidal-vision/refs/heads/main/security/tidal-vision-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Specialty Chemicals
- Materials Science
- Water Treatment
- Agriculture
- Sustainability
- Manufacturing
---
