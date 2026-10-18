---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crmbonus.com.br
  spf: true
hosts:
- cert_expires: Dec 18 16:01:34 2026 GMT
  host: www.crmbonus.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crmbonus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crmbônus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crmbônus
provider_slug: crmbonus
slug: crmbonus-domain-security
source_filename: crmbonus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crmbonus.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 16:01:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crmbonus.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crmbonus/refs/heads/main/security/crmbonus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software-as-a-Service
- Retail
- Loyalty
- Marketing
---
