---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usadata.com
  spf: true
hosts:
- cert_expires: Oct  3 23:44:52 2026 GMT
  host: www.usadata.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 16:10:40 2026 GMT
  host: leadsengine.usadata.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Usadata Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USADATA, Inc., probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: USADATA, Inc.
provider_slug: usadata-inc
slug: usadata-inc-domain-security
source_filename: usadata-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usadata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:44:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: leadsengine.usadata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 16:10:40 2026 GMT\n  hsts: null\ndomains:\n- domain: usadata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usadata-inc/refs/heads/main/security/usadata-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Marketing
- Data Enrichment
- Audience Targeting
- Data Hygiene
- Direct Mail
- Leads
- SOAP
- Mailing Lists
---
