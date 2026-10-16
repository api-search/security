---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caseblink.com
  spf: true
hosts:
- cert_expires: Dec 13 12:14:32 2026 GMT
  host: www.caseblink.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caseblink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CaseBlink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CaseBlink
provider_slug: caseblink
slug: caseblink-domain-security
source_filename: caseblink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caseblink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 12:14:32 2026 GMT\n  hsts: false\ndomains:\n- domain: caseblink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caseblink/refs/heads/main/security/caseblink-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Immigration
- LegalTech
- Automation
---
