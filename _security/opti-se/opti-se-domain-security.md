---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@opti.se"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opti.se
  spf: true
hosts:
- cert_expires: Dec 17 23:36:27 2026 GMT
  host: www.opti.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opti Se Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opti, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Opti
provider_slug: opti-se
slug: opti-se-domain-security
source_filename: opti-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opti.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:36:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opti.se\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@opti.se\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opti-se/refs/heads/main/security/opti-se-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Savings
- Investments
- Sweden
---
