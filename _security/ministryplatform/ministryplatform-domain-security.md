---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ministryplatform.com
  spf: true
hosts:
- cert_expires: Dec 27 12:51:50 2026 GMT
  host: ministryplatform.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MinistryPlatform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MinistryPlatform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MinistryPlatform
provider_slug: ministryplatform
slug: ministryplatform-domain-security
source_filename: ministryplatform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ministryplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 12:51:50 2026 GMT\n  hsts: false\ndomains:\n- domain: ministryplatform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ministryplatform/security/ministryplatform-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Church
- ManagementSoftware
- Integration
---
