---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airna.com
  spf: true
hosts:
- cert_expires: Oct 26 16:57:04 2026 GMT
  host: airna.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIRNA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AIRNA
provider_slug: airna
slug: airna-domain-security
source_filename: airna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 16:57:04 2026 GMT\n  hsts: false\ndomains:\n- domain: airna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airna/refs/heads/main/security/airna-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Therapeutics
- RNA Editing
- Genetic Medicine
- Life Sciences
- Rare Disease
- Pharmaceuticals
---
