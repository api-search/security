---
api_specs:
- filename: amazon-ads-openapi-generated.yml
  format: yaml
  label: Amazon Ads API
  slug: amazon-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ads/refs/heads/main/openapi/_ae-authored/amazon-ads-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: advertising.amazon.com
  hsts: true
  hsts_max_age: 47474747
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amazon Ads Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Ads, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Ads
provider_slug: amazon-ads
slug: amazon-ads-domain-security
source_filename: amazon-ads-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: advertising.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 47474747\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-ads/refs/heads/main/security/amazon-ads-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Marketing
- Amazon
- Technology
- SaaS
---
