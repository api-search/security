---
api_specs:
- filename: upgrade-flexpay-openapi.yml
  format: yaml
  label: Flex Pay API
  slug: flex-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrade/refs/heads/main/openapi/upgrade-flexpay-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:admin@upgrade.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: upgrade.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uplift.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.upgrade.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 03:47:07 2026 GMT
  host: docs.uplift.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: partner.upgrade.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upgrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upgrade, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Upgrade
provider_slug: upgrade
slug: upgrade-domain-security
source_filename: upgrade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.upgrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\n- host: docs.uplift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 03:47:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner.upgrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: upgrade.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:admin@upgrade.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: uplift.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upgrade/refs/heads/main/security/upgrade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Lending
- Buy Now Pay Later
- Payments
- Credit Cards
- Banking
- Travel
---
