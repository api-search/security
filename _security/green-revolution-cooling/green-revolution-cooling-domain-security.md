---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grcooling.com
  spf: true
hosts:
- cert_expires: Oct 19 17:34:13 2026 GMT
  host: www.grcooling.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Green Revolution Cooling Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Revolution Cooling, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Green Revolution Cooling
provider_slug: green-revolution-cooling
slug: green-revolution-cooling-domain-security
source_filename: green-revolution-cooling-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.grcooling.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 17:34:13 2026 GMT\n  hsts: false\ndomains:\n- domain: grcooling.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-revolution-cooling/refs/heads/main/security/green-revolution-cooling-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Centers
- Immersion Cooling
- Liquid Cooling
- Infrastructure
- Hardware
- Energy Efficiency
- High Performance Computing
- Artificial Intelligence
- Sustainability
---
