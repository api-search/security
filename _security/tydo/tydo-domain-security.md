---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tydo.com
  spf: true
hosts:
- cert_expires: Oct 13 17:42:25 2026 GMT
  host: tydo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tydo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tydo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tydo
provider_slug: tydo
slug: tydo-domain-security
source_filename: tydo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tydo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 17:42:25 2026 GMT\n  hsts: false\ndomains:\n- domain: tydo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tydo/refs/heads/main/security/tydo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Applications
- Shopify
- eCommerce
- Audits
- AI Agents
- Analytics
---
