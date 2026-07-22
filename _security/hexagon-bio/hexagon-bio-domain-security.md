---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hexagonbio.com
  spf: true
hosts:
- cert_expires: Oct 12 12:02:41 2026 GMT
  host: www.hexagonbio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hexagon Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hexagon Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hexagon Bio
provider_slug: hexagon-bio
slug: hexagon-bio-domain-security
source_filename: hexagon-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hexagonbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 12:02:41 2026 GMT\n  hsts: false\ndomains:\n- domain: hexagonbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hexagon-bio/refs/heads/main/security/hexagon-bio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Health Tech
- Biotechnology
- Oncology
- Antibody-Drug Conjugates
- Drug Discovery
- Therapeutics
---
