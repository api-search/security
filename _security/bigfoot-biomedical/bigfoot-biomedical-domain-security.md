---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bigfootbiomedical.com
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.bigfootbiomedical.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: clinichub.bigfootbiomedical.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Bigfoot Clinic Hub healthcare-professional portal, served from Salesforce Experience Cloud (siteforce.com). Added by hand; not discovered by the mechanical probe because no apis[] entry points at this host.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bigfoot Biomedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bigfoot Biomedical, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bigfoot Biomedical
provider_slug: bigfoot-biomedical
slug: bigfoot-biomedical-domain-security
source_filename: bigfoot-biomedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bigfootbiomedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: clinichub.bigfootbiomedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: Bigfoot Clinic Hub healthcare-professional portal, served from Salesforce\n    Experience Cloud (siteforce.com). Added by hand; not discovered by the mechanical\n    probe because no apis[] entry points at this host.\ndomains:\n- domain: bigfootbiomedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigfoot-biomedical/refs/heads/main/security/bigfoot-biomedical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Digital Health
- Medical Devices
- Diabetes
- Insulin Management
- Continuous Glucose Monitoring
- Connected Devices
- Acquired
---
