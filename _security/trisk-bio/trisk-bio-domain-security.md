---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: triskbio.com
  spf: true
hosts:
- cert_expires: Sep 30 20:01:09 2026 GMT
  host: triskbio.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trisk Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trisk Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Trisk Bio
provider_slug: trisk-bio
slug: trisk-bio-domain-security
source_filename: trisk-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: triskbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:01:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: triskbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trisk-bio/refs/heads/main/security/trisk-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthtech
- Biotechnology
- Gene Therapy
- AAV Manufacturing
- Biomanufacturing
- CDMO
- Preclinical
- Life Sciences
---
