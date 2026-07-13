---
api_specs:
- filename: nycu-dataverse.yaml
  format: yaml
  label: NYCU Dataverse Repository API
  slug: dataverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nycu/refs/heads/main/openapi/nycu-dataverse.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: nycu.edu.tw
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dataverse.org
  spf: true
hosts:
- host: www.nycu.edu.tw
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Missing Subject Key Identifier (_ssl.c:1082)'
- cert_expires: Sep 24 13:31:58 2026 GMT
  host: id.nycu.edu.tw
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: guides.dataverse.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nycu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Yang Ming Chiao Tung University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: National Yang Ming Chiao Tung University
provider_slug: nycu
slug: nycu-domain-security
source_filename: nycu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nycu.edu.tw\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Missing Subject\n    Key Identifier (_ssl.c:1082)'\n  hsts: null\n- host: id.nycu.edu.tw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 13:31:58 2026 GMT\n  hsts: false\n- host: guides.dataverse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: nycu.edu.tw\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: dataverse.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nycu/refs/heads/main/security/nycu-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Taiwan
- Identity
- OAuth
- Research Data
- Open Data
- Library
---
