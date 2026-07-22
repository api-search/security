---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: odaseva.com
  spf: true
hosts:
- cert_expires: Oct  8 14:16:46 2026 GMT
  host: www.odaseva.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Odaseva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Odaseva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Odaseva
provider_slug: odaseva
slug: odaseva-domain-security
source_filename: odaseva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.odaseva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 14:16:46 2026 GMT\n  hsts: false\ndomains:\n- domain: odaseva.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odaseva/refs/heads/main/security/odaseva-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Infrastructure Saas
- Salesforce
- Data Protection
- Backup
- Data Governance
- Security
- Compliance
- Privacy
---
