---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:it-systems@color.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: color.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: redoxengine.com
  spf: true
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: www.color.com
  hsts: true
  hsts_max_age: 1800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 20:13:48 2026 GMT
  host: www.redoxengine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Color Genomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Color Health, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Color Health
provider_slug: color-genomics
slug: color-genomics-domain-security
source_filename: color-genomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.color.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 1800\n- host: www.redoxengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: color.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:it-systems@color.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: redoxengine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/color-genomics/refs/heads/main/security/color-genomics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Genomics
- Genetic Testing
- Precision Health
- Population Health
- Cancer Screening
- Clinical
- Enterprise
- Gated
---
