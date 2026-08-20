---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caainsurancecompany.ca
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: caainsurance.com
  spf: false
- caa: []
  dmarc: true
  dmarc_note: _dmarc CNAMEs to caainsurancecompany.com.hosted.dmarc-report.com (managed DMARC); no policy TXT resolved anonymously
  dmarc_policy: hosted
  dnssec: false
  domain: caainsurancecompany.com
  spf: true
  spf_record: v=spf1 ip4:167.89.89.217 ip4:67.205.56.172 include:spf.caasco.ca include:spf.protection.outlook.com include:_spf.act-on.net -all
- caa: []
  dmarc: false
  dnssec: false
  domain: caabrokerportal.ca
  note: SPF hard-fails all mail (send-nothing domain); no DMARC record.
  spf: true
  spf_record: v=spf1 -all
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: caainsurancecompany.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: broker.caainsurance.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 23 23:59:59 2026 GMT
  cert_issuer: Sectigo Public Server Authentication CA OV R36
  cert_subject: CN=*.caabrokerportal.ca, O=CAA South Central Ontario Systems and Services Inc., ST=Ontario, C=CA
  host: www.caabrokerportal.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: Microsoft-IIS/10.0 (MicrosoftSharePointTeamServices 16.0.0.5552)
  tls_version: TLSv1.2
- cert_expires: Oct 30 23:59:59 2026 GMT
  csp: true
  host: customer.caainsurancecompany.ca
  hsts: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  server: ZENEDGE
  tls_version: TLSv1.3
- cert_expires: Sep 14 05:01:12 2026 GMT
  host: car-insurance.caainsurancecompany.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Sep 17 16:48:59 2026 GMT
  host: property-insurance.caainsurancecompany.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caa Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CAA Insurance, probed live across 6 host(s) and 4 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CAA Insurance
provider_slug: caa-insurance
slug: caa-insurance-domain-security
source_filename: caa-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caainsurancecompany.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: broker.caainsurance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: null\n- host: www.caabrokerportal.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  cert_issuer: Sectigo Public Server Authentication CA OV R36\n  cert_subject: CN=*.caabrokerportal.ca, O=CAA South Central Ontario Systems and Services Inc., ST=Ontario, C=CA\n  hsts: true\n  hsts_max_age: 31536000\n  server: Microsoft-IIS/10.0 (MicrosoftSharePointTeamServices 16.0.0.5552)\n- host: customer.caainsurancecompany.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_preload: true\n  csp:\
  \ true\n  server: ZENEDGE\n- host: car-insurance.caainsurancecompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:01:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  server: cloudflare\n- host: property-insurance.caainsurancecompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:48:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  server: cloudflare\ndomains:\n- domain: caainsurancecompany.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: caainsurance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: caainsurancecompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 ip4:167.89.89.217 ip4:67.205.56.172 include:spf.caasco.ca include:spf.protection.outlook.com include:_spf.act-on.net -all'\n  dmarc: true\n  dmarc_policy: hosted\n  dmarc_note: _dmarc CNAMEs to caainsurancecompany.com.hosted.dmarc-report.com\
  \ (managed DMARC); no policy TXT resolved anonymously\n- domain: caabrokerportal.ca\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 -all\n  dmarc: false\n  note: SPF hard-fails all mail (send-nothing domain); no DMARC record.\ndetail:\n  dmarc_caainsurancecompany_ca: 'v=DMARC1; p=none; fo=1; rua=mailto:0cd63e3c@mxtoolbox.dmarc-report.com; ruf=mailto:0cd63e3c@forensics.dmarc-report.com;'\n  spf_caainsurancecompany_ca: 'v=spf1 include:spf.caasco.ca include:spf.protection.outlook.com -all'\n  probed_extra: '2026-07-25 — customer portal, broker portal, and both quote applications probed manually and added to hosts[]'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caa-insurance/refs/heads/main/security/caa-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Canada
- Property and Casualty
- Auto Insurance
- Home Insurance
- Carrier
- Brokers
- Personal Lines
- Telematics
- Partner Gated
- No Public API
---
