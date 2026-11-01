---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: earthscope.org
  spf: true
hosts:
- cert_expires: May  5 23:59:59 2027 GMT
  host: www.earthscope.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Earthscope Consortium Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EarthScope Consortium, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EarthScope Consortium, Inc.
provider_slug: earthscope-consortium-inc
slug: earthscope-consortium-inc-domain-security
source_filename: earthscope-consortium-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.earthscope.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: earthscope.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/earthscope-consortium-inc/security/earthscope-consortium-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geophysics
- Research
- Education
- NSF
---
