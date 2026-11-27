---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:dmarc@alphaassay.com"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alphaassay.com
  spf: true
hosts:
- cert_expires: Dec  2 13:02:38 2026 GMT
  host: alphaassay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AlphaAssay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlphaAssay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AlphaAssay
provider_slug: alphaassay-com
slug: alphaassay-com-domain-security
source_filename: alphaassay-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alphaassay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 13:02:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alphaassay.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:dmarc@alphaassay.com\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/alphaassay-com/security/alphaassay-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Trading
- Artificial Intelligence
- Validation
---
