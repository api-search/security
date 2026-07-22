---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kronosbio.com
  spf: true
hosts:
- cert_expires: Jan  2 19:01:52 2027 GMT
  host: kronosbio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kronos Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kronos Bio *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kronos Bio *
provider_slug: kronos-bio
slug: kronos-bio-domain-security
source_filename: kronos-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kronosbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 19:01:52 2027 GMT\n  hsts: false\ndomains:\n- domain: kronosbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kronos-bio/refs/heads/main/security/kronos-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Oncology
- Pharmaceuticals
- Drug Discovery
---
