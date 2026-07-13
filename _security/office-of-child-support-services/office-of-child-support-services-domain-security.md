---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "e5.com"
  - 0 issue "entrust.net"
  - 0 issue "globalsign.com"
  - 0 issue "identrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hhs.gov
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: www.acf.hhs.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Office Of Child Support Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Office of Child Support Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Office of Child Support Services
provider_slug: office-of-child-support-services
slug: office-of-child-support-services-domain-security
source_filename: office-of-child-support-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acf.hhs.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: hhs.gov\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"e5.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/office-of-child-support-services/refs/heads/main/security/office-of-child-support-services-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Federal Government
---
