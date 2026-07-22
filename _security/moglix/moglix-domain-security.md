---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moglix.com
  spf: true
hosts:
- cert_expires: Oct 10 08:43:07 2026 GMT
  host: www.moglix.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moglix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moglix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moglix
provider_slug: moglix
slug: moglix-domain-security
source_filename: moglix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moglix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 08:43:07 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: moglix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moglix/refs/heads/main/security/moglix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplaces
- B2B
- Ecommerce
- Procurement
- Industrial Supplies
- Supply Chain
- India
---
