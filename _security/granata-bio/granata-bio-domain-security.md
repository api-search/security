---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: granata.bio
  spf: true
hosts:
- cert_expires: Oct  3 17:14:57 2026 GMT
  host: www.granata.bio
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Granata Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Granata Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Granata Bio
provider_slug: granata-bio
slug: granata-bio-domain-security
source_filename: granata-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.granata.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:14:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: granata.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granata-bio/refs/heads/main/security/granata-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Biopharmaceutical
- Reproductive Health
- Fertility
- Women's Health
- IVF
- Clinical Trials
- Healthcare
---
