---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: salesforce.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.salesforce.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: developer.salesforce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: <short-code>.api.commercecloud.salesforce.com
  https: false
kind: domain-security
layout: security
method: probed
name: Salesforce Commerce Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesforce Commerce Cloud, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salesforce Commerce Cloud
provider_slug: salesforce-commerce-cloud
slug: salesforce-commerce-cloud-domain-security
source_filename: salesforce-commerce-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: developer.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: <short-code>.api.commercecloud.salesforce.com\n  https: false\ndomains:\n- domain: salesforce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-commerce-cloud/refs/heads/main/security/salesforce-commerce-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Commerce
- E-Commerce
- Headless Commerce
- Salesforce
- B2C Commerce
- B2B Commerce
- Demandware
---
