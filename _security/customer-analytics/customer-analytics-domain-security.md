---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: customeranalytics.com
  spf: true
hosts:
- cert_expires: Dec 18 06:31:33 2026 GMT
  host: www.customeranalytics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Customer Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Customer Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Customer Analytics
provider_slug: customer-analytics
slug: customer-analytics-domain-security
source_filename: customer-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.customeranalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 06:31:33 2026 GMT\n  hsts: false\ndomains:\n- domain: customeranalytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customer-analytics/refs/heads/main/security/customer-analytics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Data
- Artificial Intelligence
- Machine Learning
- Business Intelligence
- Data Engineering
- Quality Assurance
- Internet of Things
- Consulting
- Company
---
