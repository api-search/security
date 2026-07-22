---
api_specs:
- filename: wegalvanize-highbond-openapi-original.yml
  format: yaml
  label: HighBond API
  slug: highbond-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegalvanize/refs/heads/main/openapi/wegalvanize-highbond-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wegalvanize.com
  spf: true
- caa:
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: highbond.com
  spf: true
hosts:
- host: wegalvanize.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''wegalvanize'
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: docs-apis.highbond.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: apis-us.highbond.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wegalvanize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wegalvanize, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wegalvanize
provider_slug: wegalvanize
slug: wegalvanize-domain-security
source_filename: wegalvanize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wegalvanize.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''wegalvanize'\n  hsts: null\n- host: docs-apis.highbond.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\n- host: apis-us.highbond.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: wegalvanize.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: highbond.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wegalvanize/refs/heads/main/security/wegalvanize-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Governance
- Risk
- Compliance
- Audit
- GRC
- Analytics
- Automation
- Security
---
