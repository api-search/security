---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: revaliabio.com
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: revaliabio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revalia Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revalia Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Revalia Bio
provider_slug: revalia-bio
slug: revalia-bio-domain-security
source_filename: revalia-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revaliabio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: revaliabio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revalia-bio/refs/heads/main/security/revalia-bio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotech
- AI
- Drug Development
- Medical Devices
- Clinical Data
- Life Sciences
- Translational Science
---
