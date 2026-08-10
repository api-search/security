---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mitiga.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mitiga.cloud
  spf: true
hosts:
- cert_expires: Sep 10 04:14:27 2026 GMT
  host: www.mitiga.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: api.mitiga.cloud
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mitiga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mitiga, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mitiga
provider_slug: mitiga
slug: mitiga-domain-security
source_filename: mitiga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mitiga.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 04:14:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mitiga.cloud\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mitiga.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mitiga.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mitiga/refs/heads/main/security/mitiga-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cloud Security
- SaaS Security
- Cloud Detection and Response
- Incident Response
- Threat Detection
- Identity Security
- Managed Security Services
- Artificial Intelligence
---
