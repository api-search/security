---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: convercent.com
  spf: true
hosts:
- cert_expires: Sep 22 06:16:15 2026 GMT
  host: www.convercent.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Convercent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Convercent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Convercent
provider_slug: convercent
slug: convercent-domain-security
source_filename: convercent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.convercent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 06:16:15 2026 GMT\n  hsts: false\ndomains:\n- domain: convercent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convercent/refs/heads/main/security/convercent-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Saas
- Compliance
- Governance Risk And Compliance
- Ethics
- Case Management
- OData
- Reporting
---
