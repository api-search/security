---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: swag.com
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: swag.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swagcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swag.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Swag.com
provider_slug: swagcom
slug: swagcom-domain-security
source_filename: swagcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: swag.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swagcom/refs/heads/main/security/swagcom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Promotional Products
- Branded Merchandise
- Swag
- E-commerce
- Custom Products
- Fulfillment
---
