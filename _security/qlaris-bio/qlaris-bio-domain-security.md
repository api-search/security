---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qlaris.bio
  spf: true
hosts:
- cert_expires: Aug 31 16:24:07 2026 GMT
  host: qlaris.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qlaris Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qlaris Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qlaris Bio
provider_slug: qlaris-bio
slug: qlaris-bio-domain-security
source_filename: qlaris-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qlaris.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:24:07 2026 GMT\n  hsts: false\ndomains:\n- domain: qlaris.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qlaris-bio/refs/heads/main/security/qlaris-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Ophthalmology
- Glaucoma
- Clinical Stage
- Life Sciences
- Healthcare
---
