---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: owasp.org
  spf: true
hosts:
- cert_expires: Oct  6 05:06:52 2026 GMT
  host: owasp.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Owasp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OWASP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OWASP
provider_slug: owasp
slug: owasp-domain-security
source_filename: owasp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: owasp.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:06:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: owasp.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owasp/refs/heads/main/security/owasp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Security
- Open Source
- Security
- Web Security
- Standards
---
