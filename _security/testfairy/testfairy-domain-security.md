---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: testfairy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: saucelabs.com
  spf: true
hosts:
- cert_expires: Aug 14 23:59:59 2026 GMT
  host: testfairy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 20:07:48 2026 GMT
  host: docs.saucelabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: mobile.saucelabs.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Testfairy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TestFairy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TestFairy
provider_slug: testfairy
slug: testfairy-domain-security
source_filename: testfairy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: testfairy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.saucelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 20:07:48 2026 GMT\n  hsts: false\n- host: mobile.saucelabs.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: testfairy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: saucelabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testfairy/refs/heads/main/security/testfairy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile
- Testing
- App Distribution
- Beta Testing
- Quality Assurance
- Developer Tools
- Session Recording
- Crash Reporting
- DevOps
---
