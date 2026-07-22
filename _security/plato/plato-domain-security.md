---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: platohq.com
  spf: true
hosts:
- cert_expires: Sep  1 23:11:11 2026 GMT
  host: www.platohq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plato, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Plato
provider_slug: plato
slug: plato-domain-security
source_filename: plato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.platohq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:11:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: platohq.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plato/refs/heads/main/security/plato-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Applicative Saas
- Mentorship
- Engineering Leadership
- Community
- Deactivated
- Deactivated Company
---
