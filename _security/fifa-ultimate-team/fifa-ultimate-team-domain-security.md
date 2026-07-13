---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: easports.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.easports.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fifa Ultimate Team Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FIFA Ultimate Team, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FIFA Ultimate Team
provider_slug: fifa-ultimate-team
slug: fifa-ultimate-team-domain-security
source_filename: fifa-ultimate-team-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.easports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: easports.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fifa-ultimate-team/refs/heads/main/security/fifa-ultimate-team-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Games And Comics
- Public APIs
---
