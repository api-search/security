---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: symplr.com
  spf: true
hosts:
- cert_expires: Nov 10 14:57:13 2026 GMT
  host: www.symplr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Symplr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for symplr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: symplr
provider_slug: symplr
slug: symplr-domain-security
source_filename: symplr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.symplr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 14:57:13 2026 GMT\n  hsts: false\ndomains:\n- domain: symplr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symplr/refs/heads/main/security/symplr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Healthcare Operations
- Provider Data Management
- Credentialing
- Workforce Management
- Compliance
- Supply Chain
---
