---
api_specs:
- filename: activecampaign-api-v3
  format: yaml
  label: ActiveCampaign API v3
  slug: api-v3
  spec_type: Postman
  url: https://www.postman.com/acdevrel/activecampaign-developer-relations/collection/ju5a59q/activecampaign-api-v3
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
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: www.activecampaign.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
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
name: Active Campaign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ActiveCampaign, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ActiveCampaign
provider_slug: active-campaign
slug: active-campaign-domain-security
source_filename: active-campaign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.activecampaign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.activecampaign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:54:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: youraccountname.api-us1.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 14 02:58:32 2026 GMT\n  hsts: null\ndomains:\n- domain: activecampaign.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: api-us1.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/security/active-campaign-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing Automation
- Email Marketing
- CRM
- Customer Experience Automation
- Sales Engagement
---
