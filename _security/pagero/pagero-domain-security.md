---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pagero.com
  spf: true
hosts:
- cert_expires: Dec  1 09:03:01 2026 GMT
  host: www.pagero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pagero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pagero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pagero
provider_slug: pagero
slug: pagero-domain-security
source_filename: pagero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pagero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 09:03:01 2026 GMT\n  hsts: false\ndomains:\n- domain: pagero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagero/refs/heads/main/security/pagero-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- e-invoicing
- AP Automation
- Compliance
- B2B
---
