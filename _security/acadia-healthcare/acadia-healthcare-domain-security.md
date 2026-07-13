---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acadiahealthcare.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.acadiahealthcare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.acadiahealthcare.com
  https: false
- cert_expires: Dec 13 15:59:27 2026 GMT
  host: api.acadiahealthcare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acadia Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acadia Healthcare, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acadia Healthcare
provider_slug: acadia-healthcare
slug: acadia-healthcare-domain-security
source_filename: acadia-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acadiahealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\n- host: developer.acadiahealthcare.com\n  https: false\n- host: api.acadiahealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 15:59:27 2026 GMT\n  hsts: null\ndomains:\n- domain: acadiahealthcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acadia-healthcare/refs/heads/main/security/acadia-healthcare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Behavioral Health
- Mental Health
---
