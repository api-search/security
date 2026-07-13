---
api_specs:
- filename: Welcome.html
  format: yaml
  label: Amazon QuickSight API
  slug: amazon-quicksight-api
  spec_type: OpenAPI
  url: https://docs.aws.amazon.com/quicksight/latest/APIReference/Welcome.html
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: quicksight.aws.amazon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: quicksight.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Quicksight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon QuickSight, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon QuickSight
provider_slug: amazon-quicksight
slug: amazon-quicksight-domain-security
source_filename: amazon-quicksight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quicksight.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: quicksight.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-quicksight/refs/heads/main/security/amazon-quicksight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- BI
- Business Intelligence
- Dashboards
- Machine Learning
- Reporting
- Visualization
---
