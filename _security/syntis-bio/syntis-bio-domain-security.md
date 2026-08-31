---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: syntis.bio
  spf: true
hosts:
- cert_expires: Oct 28 17:03:05 2026 GMT
  host: syntis.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Syntis Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syntis Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Syntis Bio
provider_slug: syntis-bio
slug: syntis-bio-domain-security
source_filename: syntis-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syntis.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 17:03:05 2026 GMT\n  hsts: false\ndomains:\n- domain: syntis.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syntis-bio/refs/heads/main/security/syntis-bio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Drug Delivery
- Clinical Stage
- Obesity
- Rare Disease
- Health
---
