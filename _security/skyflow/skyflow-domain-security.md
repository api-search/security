---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: skyflow.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: skyflowapis.com
  spf: false
hosts:
- cert_expires: Sep 10 23:23:11 2026 GMT
  host: www.skyflow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 15:18:39 2026 GMT
  host: docs.skyflow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 07:31:38 2026 GMT
  host: manage.skyflowapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skyflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skyflow, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Skyflow
provider_slug: skyflow
slug: skyflow-domain-security
source_filename: skyflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skyflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:23:11 2026 GMT\n  hsts: false\n- host: docs.skyflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:18:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: manage.skyflowapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 07:31:38 2026 GMT\n  hsts: null\ndomains:\n- domain: skyflow.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: skyflowapis.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyflow/refs/heads/main/security/skyflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data Privacy
- PII
- Tokenization
- Data Security
- Vault
- Compliance
- PCI
- Encryption
- Data Governance
---
