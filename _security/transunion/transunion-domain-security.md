---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: transunion.com
  spf: true
hosts:
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: www.transunion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.transunion.com
  https: false
kind: domain-security
layout: security
method: probed
name: Transunion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TransUnion, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TransUnion
provider_slug: transunion
slug: transunion-domain-security
source_filename: transunion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transunion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: null\n- host: developer.transunion.com\n  https: false\ndomains:\n- domain: transunion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transunion/refs/heads/main/security/transunion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial
- Credit Reporting
- Risk
- Identity
- Fraud
- Marketing
---
