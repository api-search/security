---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: authorea.com
  spf: true
hosts:
- cert_expires: Oct  2 12:11:49 2026 GMT
  host: www.authorea.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Authorea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Authorea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Authorea
provider_slug: authorea
slug: authorea-domain-security
source_filename: authorea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.authorea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:11:49 2026 GMT\n  hsts: null\ndomains:\n- domain: authorea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authorea/refs/heads/main/security/authorea-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Scholarly Publishing
- Academic Writing
- Collaboration
- Research
- Preprints
- LaTeX
- Wiley
---
