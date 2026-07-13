---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: polimi.it
  spf: true
hosts:
- cert_expires: Nov 25 15:12:43 2026 GMT
  host: www.polimi.it
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 13:14:43 2026 GMT
  host: re.public.polimi.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 01:00:39 2026 GMT
  host: opendata.polimi.it
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Politecnico Di Milano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Politecnico di Milano, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Politecnico di Milano
provider_slug: politecnico-di-milano
slug: politecnico-di-milano-domain-security
source_filename: politecnico-di-milano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.polimi.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 15:12:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: re.public.polimi.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 13:14:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: opendata.polimi.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 01:00:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: polimi.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-milano/refs/heads/main/security/politecnico-di-milano-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Repository
- OAI-PMH
- Identity
- Italy
---
