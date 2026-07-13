---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: certinia.com
  note: SPF includes _spf.salesforce.com, consistent with Certinia's Salesforce-native delivery model. The apex domain (certinia.com) did not return an HSTS header on probe, while www and help subdomains do.
  spf: true
  spf_record: v=spf1 ip4:52.38.191.241 ip4:83.138.173.144 include:eu._netblocks.mimecast.com include:mktomail.com include:_spf.salesforce.com include:_spf.google.com include:em9009.seismic.com -all
hosts:
- cert_expires: Oct  2 10:44:29 2026 GMT
  host: certinia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 17:41:13 2026 GMT
  host: www.certinia.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 09:30:32 2026 GMT
  host: help.certinia.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Certinia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certinia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Certinia
provider_slug: certinia
slug: certinia-domain-security
source_filename: certinia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts\nhosts:\n- host: certinia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 10:44:29 2026 GMT\n  hsts: false\n- host: www.certinia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 17:41:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: help.certinia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 09:30:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: certinia.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 ip4:52.38.191.241 ip4:83.138.173.144 include:eu._netblocks.mimecast.com include:mktomail.com include:_spf.salesforce.com include:_spf.google.com include:em9009.seismic.com -all'\n  dmarc: true\n  dmarc_policy: reject\n  note: >-\n    SPF includes _spf.salesforce.com, consistent with Certinia's Salesforce-native\n\
  \    delivery model. The apex domain (certinia.com) did not return an HSTS header on\n    probe, while www and help subdomains do.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certinia/refs/heads/main/security/certinia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Revenue Recognition
- ASC 606
- ERP
- Professional Services Automation
- PSA
- Billing
- Accounting
- Salesforce
- FinancialForce
- Finance
---
