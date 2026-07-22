---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: usadata.com
  spf: true
hosts:
- cert_expires: Oct  3 23:44:52 2026 GMT
  host: www.usadata.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usadata Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USADATA, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: USADATA, Inc.
provider_slug: usadata-inc
slug: usadata-inc-domain-security
source_filename: usadata-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usadata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:44:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: usadata.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usadata-inc/refs/heads/main/security/usadata-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data
- Marketing
- Data Enrichment
- Audience Targeting
- Data Hygiene
- Direct Mail
- Leads
---
