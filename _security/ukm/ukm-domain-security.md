---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ukm.my
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: www.ukm.my
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: ptsldigital.ukm.my
  https: false
- host: journalarticle.ukm.my
  https: false
kind: domain-security
layout: security
method: probed
name: Ukm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universiti Kebangsaan Malaysia, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Universiti Kebangsaan Malaysia
provider_slug: ukm
slug: ukm-domain-security
source_filename: ukm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ukm.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ptsldigital.ukm.my\n  https: false\n- host: journalarticle.ukm.my\n  https: false\ndomains:\n- domain: ukm.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ukm/refs/heads/main/security/ukm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Institutional Repository
- OAI-PMH
- Library
- Malaysia
---
