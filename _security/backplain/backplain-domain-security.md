---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: backplain.com
  spf: true
hosts:
- cert_expires: Nov 26 16:07:31 2026 GMT
  host: backplain.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Backplain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Backplain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Backplain
provider_slug: backplain
slug: backplain-domain-security
source_filename: backplain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: backplain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 16:07:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: backplain.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backplain/refs/heads/main/security/backplain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Data Governance
- Security
- Enterprise
---
