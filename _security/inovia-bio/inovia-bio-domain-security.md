---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: inovia.bio
  spf: true
hosts:
- cert_expires: Oct  1 18:44:37 2026 GMT
  host: inovia.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inovia Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inovia Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Inovia Bio
provider_slug: inovia-bio
slug: inovia-bio-domain-security
source_filename: inovia-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inovia.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:44:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: inovia.bio\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inovia-bio/refs/heads/main/security/inovia-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- TechBio
- Biotechnology
- Pharmaceutical
- Drug Development
- Clinical Trials
- Real World Evidence
- Regulatory Strategy
---
