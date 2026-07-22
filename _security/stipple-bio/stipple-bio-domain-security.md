---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: stipple.bio
  spf: true
hosts:
- cert_expires: Sep  1 14:13:49 2026 GMT
  host: stipple.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stipple Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stipple Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Stipple Bio
provider_slug: stipple-bio
slug: stipple-bio-domain-security
source_filename: stipple-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stipple.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 14:13:49 2026 GMT\n  hsts: false\ndomains:\n- domain: stipple.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stipple-bio/refs/heads/main/security/stipple-bio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Life Sciences
- Biotechnology
- Oncology
- Precision Medicine
- Drug Discovery
- Therapeutics
- Antibody-Drug Conjugates
---
