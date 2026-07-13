---
api_specs:
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Causes API
  slug: benevity-causes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Giving API
  slug: benevity-giving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Receipts API
  slug: benevity-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Spark Giving Opportunities API
  slug: benevity-spark-giving-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Spark Volunteer Opportunities API
  slug: benevity-spark-volunteer-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: benevity.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: benevity.org
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: benevity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: developer.benevity.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: skyline.benevity.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Benevity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Benevity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Benevity
provider_slug: benevity
slug: benevity-domain-security
source_filename: benevity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: benevity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\n- host: developer.benevity.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\n- host: skyline.benevity.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: benevity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: benevity.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/security/benevity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Corporate Social Responsibility
- Workplace Giving
- Donations
- Volunteering
- Nonprofits
- Matching Gifts
- CSR
- ESG
---
