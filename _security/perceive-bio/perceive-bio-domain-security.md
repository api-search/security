---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: perceivebio.com
  spf: true
hosts:
- cert_expires: Sep 14 09:24:58 2026 GMT
  host: perceivebio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perceive Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perceive Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Perceive Bio
provider_slug: perceive-bio
slug: perceive-bio-domain-security
source_filename: perceive-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perceivebio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:24:58 2026 GMT\n  hsts: false\ndomains:\n- domain: perceivebio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perceive-bio/refs/heads/main/security/perceive-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Ophthalmology
- Therapeutics
- Retinal Degeneration
- Drug Development
- Neuroprotection
---
