---
api_specs:
- filename: owasp-zap-openapi.yml
  format: yaml
  label: OWASP ZAP API
  slug: owasp-zap
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/owasp-zap/refs/heads/main/openapi/owasp-zap-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zaproxy.org
  spf: true
hosts:
- cert_expires: Sep  1 07:18:49 2026 GMT
  host: www.zaproxy.org
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Owasp Zap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OWASP ZAP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OWASP ZAP
provider_slug: owasp-zap
slug: owasp-zap-domain-security
source_filename: owasp-zap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zaproxy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:18:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: zaproxy.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owasp-zap/refs/heads/main/security/owasp-zap-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Security Testing
- Application Security
- Vulnerability Scanning
- Testing
- Open Source
---
