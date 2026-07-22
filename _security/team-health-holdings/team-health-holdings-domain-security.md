---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teamhealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teamhealthcareers.com
  spf: true
hosts:
- cert_expires: Aug 11 19:18:28 2026 GMT
  host: www.teamhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: www.teamhealthcareers.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Team Health Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Team Health Holdings, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Team Health Holdings
provider_slug: team-health-holdings
slug: team-health-holdings-domain-security
source_filename: team-health-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teamhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 19:18:28 2026 GMT\n  hsts: false\n- host: www.teamhealthcareers.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: teamhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: teamhealthcareers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/team-health-holdings/refs/heads/main/security/team-health-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Physician Staffing
- Hospital Services
- Emergency Medicine
- Hospital Medicine
- Critical Care
- Fortune 1000
---
