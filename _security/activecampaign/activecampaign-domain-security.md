---
api_specs:
- filename: activecampaign-v3.json
  format: json
  label: ActiveCampaign API v3
  slug: activecampaign-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/openapi/activecampaign-v3.json
- filename: activecampaign-sms.json
  format: json
  label: ActiveCampaign SMS Broadcast API
  slug: activecampaign-sms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/openapi/activecampaign-sms.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: activecampaign.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: api-us1.com
  spf: false
hosts:
- cert_expires: Oct  2 15:54:45 2026 GMT
  host: developers.activecampaign.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 02:58:32 2026 GMT
  host: youraccountname.api-us1.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Activecampaign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ActiveCampaign, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ActiveCampaign
provider_slug: activecampaign
slug: activecampaign-domain-security
source_filename: activecampaign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.activecampaign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:54:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: youraccountname.api-us1.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 14 02:58:32 2026 GMT\n  hsts: null\ndomains:\n- domain: activecampaign.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: api-us1.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/security/activecampaign-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
---
