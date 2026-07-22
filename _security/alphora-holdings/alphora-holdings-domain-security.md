---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alphoraholdings.com
  spf: true
hosts:
- cert_expires: Sep 21 14:43:01 2026 GMT
  host: alphoraholdings.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alphora Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alphora Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alphora Holdings
provider_slug: alphora-holdings
slug: alphora-holdings-domain-security
source_filename: alphora-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alphoraholdings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:43:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alphoraholdings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphora-holdings/refs/heads/main/security/alphora-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Artificial Intelligence
- Managed IT Services
- IT Operations
- Cybersecurity
- Compliance
- Managed Service Providers
- Germany
---
