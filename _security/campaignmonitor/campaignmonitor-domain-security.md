---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Campaign Monitor API
  slug: campaign-monitor-api
  spec_type: OpenAPI
  url: https://www.campaignmonitor.com/api/
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issue "geotrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: campaignmonitor.com
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: createsend.com
  spf: true
hosts:
- cert_expires: Aug 18 12:31:01 2026 GMT
  host: www.campaignmonitor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 05:47:35 2026 GMT
  host: api.createsend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Campaignmonitor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Campaign Monitor, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Campaign Monitor
provider_slug: campaignmonitor
slug: campaignmonitor-domain-security
source_filename: campaignmonitor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.campaignmonitor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 12:31:01 2026 GMT\n  hsts: false\n- host: api.createsend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 05:47:35 2026 GMT\n  hsts: null\ndomains:\n- domain: campaignmonitor.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: createsend.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campaignmonitor/refs/heads/main/security/campaignmonitor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email Marketing
- Campaigns
- Subscribers
- Transactional Email
- Segments
- Newsletters
- Automation
---
