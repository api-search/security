---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: angitiabio.com
  spf: true
hosts:
- cert_expires: Oct 27 12:00:41 2026 GMT
  host: www.angitiabio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Angitia Biopharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angitia Biopharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Angitia Biopharmaceuticals
provider_slug: angitia-biopharmaceuticals
slug: angitia-biopharmaceuticals-domain-security
source_filename: angitia-biopharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.angitiabio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 12:00:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: angitiabio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angitia-biopharmaceuticals/refs/heads/main/security/angitia-biopharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Biopharmaceuticals
- Pharmaceuticals
- Life Sciences
- Drug Development
- Clinical Trials
- Healthcare
- Musculoskeletal
- Therapeutics
---
