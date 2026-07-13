---
api_specs:
- filename: hmrc-vat-mtd-openapi.yml
  format: yaml
  label: HMRC VAT (Making Tax Digital) API
  slug: hmrc-vat-mtd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hmrc/refs/heads/main/openapi/hmrc-vat-mtd-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hmrc.gov.uk
  spf: true
- caa:
  - www-cdn.production.govuk.service.gov.uk.
  - www-gov-uk.map.fastly.net.
  dmarc: false
  dnssec: true
  domain: www.gov.uk
  spf: false
hosts:
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: developer.service.hmrc.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 22:06:14 2026 GMT
  host: www.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: api.service.hmrc.gov.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hmrc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HMRC UK Tax Authority, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HMRC UK Tax Authority
provider_slug: hmrc
slug: hmrc-domain-security
source_filename: hmrc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.service.hmrc.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 22:06:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.service.hmrc.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hmrc.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: www.gov.uk\n  dnssec: true\n  caa:\n  - www-cdn.production.govuk.service.gov.uk.\n  - www-gov-uk.map.fastly.net.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hmrc/refs/heads/main/security/hmrc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Making Tax Digital
- Regulatory
- Tax
- UK
---
