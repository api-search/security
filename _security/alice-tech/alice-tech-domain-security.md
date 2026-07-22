---
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: alicetechnologies.com
  spf: true
hosts:
- cert_expires: Sep  3 19:42:06 2026 GMT
  host: www.alicetechnologies.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alice Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ALICE Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ALICE Technologies
provider_slug: alice-tech
slug: alice-tech-domain-security
source_filename: alice-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alicetechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:42:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alicetechnologies.com\n  dnssec: true\n  caa:\n  - 0 issuewild \";\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alice-tech/refs/heads/main/security/alice-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Construction
- Construction Technology
- Scheduling
- Generative Scheduling
- Construction Optioneering
- Project Planning
- BIM
- Primavera P6
- Microsoft Project
- Schedule Optimization
- DCMA 14-Point
- AI
- LLM
- Capital Projects
- Infrastructure
- Industrial Construction
---
