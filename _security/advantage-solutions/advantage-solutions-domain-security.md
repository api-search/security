---
api_specs:
- filename: advantage-solutions-youradv-content-openapi.yml
  format: yaml
  label: Advantage Solutions Corporate Content API (WordPress REST)
  slug: youradv-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advantage-solutions/refs/heads/main/openapi/advantage-solutions-youradv-content-openapi.yml
- filename: advantage-solutions-mrktblog-content-openapi.yml
  format: yaml
  label: MRKT Blog Content API (WordPress REST)
  slug: mrktblog-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advantage-solutions/refs/heads/main/openapi/advantage-solutions-mrktblog-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: advantagesolutions.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: youradv.com
  spf: true
hosts:
- cert_expires: Oct 24 05:44:26 2026 GMT
  host: www.advantagesolutions.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 05:42:15 2026 GMT
  host: youradv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:17:28 2026 GMT
  host: mrktblog.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Advantage Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advantage Solutions, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Advantage Solutions
provider_slug: advantage-solutions
slug: advantage-solutions-domain-security
source_filename: advantage-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.advantagesolutions.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 05:44:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: youradv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 05:42:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mrktblog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:17:28 2026 GMT\n  hsts: false\ndomains:\n- domain: advantagesolutions.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: youradv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advantage-solutions/refs/heads/main/security/advantage-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales
- Marketing
- Merchandising
- Consumer Goods
- Retail
- Shopper Insights
- Content
- Fortune 500
---
