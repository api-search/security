---
description: ''
domains:
- caa: []
  caa_evidence: no CAA record returned for synyi.com
  dmarc: false
  dmarc_evidence: no TXT record returned for _dmarc.synyi.com
  dnssec: false
  dnssec_evidence: no DS record returned for synyi.com
  domain: synyi.com
  mx:
  - ' 1 synyi-com.mail.protection.partner.outlook.cn.'
  spf: true
  spf_note: Hard-fail (-all) policy delegating to Microsoft 365 operated by 21Vianet (the China instance), consistent with the MX record synyi-com.mail.protection.partner.outlook.cn.
  spf_record: v=spf1 include:spf.protection.partner.outlook.cn -all
hosts:
- findings:
  - No Strict-Transport-Security header is returned, so a first-contact downgrade is possible even though HTTP does redirect to HTTPS.
  - The Server header discloses an exact software version (Apache/2.4.54, Debian), which is unnecessary version disclosure.
  - A wildcard certificate (*.synyi.com) is combined with wildcard DNS, so every subdomain — including api., open., developer., docs., mcp. — presents a valid certificate regardless of whether a service exists behind it. api.synyi.com answers 503 and open.synyi.com serves the stock nginx default page, both under a trusted certificate.
  host: www.synyi.com
  hsts: false
  hsts_header: null
  http_status: 200
  http_to_https_redirect: true
  http_version: '2'
  https: true
  redirect_evidence: http://www.synyi.com/ returns 301 to https://www.synyi.com:443/
  server_header: Apache/2.4.54 (Debian)
  tls_certificate:
    not_after: '2027-01-01'
    not_before: '2025-12-04'
    subject: CN=*.synyi.com
    wildcard: true
  tls_verify_result: 0
- findings:
  - nginx vhost resolving via wildcard DNS with no upstream; returns 503 on every path probed.
  host: api.synyi.com
  http_status: 503
  https: true
  tls_certificate:
    not_after: '2027-01-01'
    subject: CN=*.synyi.com
    wildcard: true
- findings:
  - Serves the stock "Welcome to nginx!" default page (612 bytes); an unconfigured vhost.
  host: open.synyi.com
  http_status: 200
  https: true
  tls_certificate:
    not_after: '2027-01-01'
    subject: CN=*.synyi.com
    wildcard: true
kind: domain-security
layout: security
method: probed
name: Synyi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synyi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Synyi
provider_slug: synyi
slug: synyi-domain-security
source_filename: synyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of www.synyi.com and synyi.com, 2026-08-29\nnote: >-\n  The automated probe initially recorded https:false for www.synyi.com. That was a false\n  negative caused by request timeouts against a China-hosted origin — the host is reachable\n  but slow and intermittently unresponsive from US vantage points. Re-probed by hand: HTTPS\n  is served correctly over HTTP/2 with a valid certificate. Every value below was verified\n  directly and the header/record evidence is recorded alongside it.\nhosts:\n- host: www.synyi.com\n  https: true\n  http_status: 200\n  http_version: '2'\n  tls_verify_result: 0\n  tls_certificate:\n    subject: CN=*.synyi.com\n    not_before: '2025-12-04'\n    not_after: '2027-01-01'\n    wildcard: true\n  hsts: false\n  hsts_header: null\n  http_to_https_redirect: true\n  redirect_evidence: http://www.synyi.com/ returns 301 to https://www.synyi.com:443/\n  server_header: Apache/2.4.54\
  \ (Debian)\n  findings:\n  - >-\n    No Strict-Transport-Security header is returned, so a first-contact downgrade is possible\n    even though HTTP does redirect to HTTPS.\n  - >-\n    The Server header discloses an exact software version (Apache/2.4.54, Debian), which is\n    unnecessary version disclosure.\n  - >-\n    A wildcard certificate (*.synyi.com) is combined with wildcard DNS, so every subdomain —\n    including api., open., developer., docs., mcp. — presents a valid certificate regardless\n    of whether a service exists behind it. api.synyi.com answers 503 and open.synyi.com serves\n    the stock nginx default page, both under a trusted certificate.\n- host: api.synyi.com\n  https: true\n  http_status: 503\n  tls_certificate:\n    subject: CN=*.synyi.com\n    not_after: '2027-01-01'\n    wildcard: true\n  findings:\n  - nginx vhost resolving via wildcard DNS with no upstream; returns 503 on every path probed.\n- host: open.synyi.com\n  https: true\n  http_status: 200\n  tls_certificate:\n\
  \    subject: CN=*.synyi.com\n    not_after: '2027-01-01'\n    wildcard: true\n  findings:\n  - Serves the stock \"Welcome to nginx!\" default page (612 bytes); an unconfigured vhost.\ndomains:\n- domain: synyi.com\n  dnssec: false\n  dnssec_evidence: no DS record returned for synyi.com\n  caa: []\n  caa_evidence: no CAA record returned for synyi.com\n  spf: true\n  spf_record: v=spf1 include:spf.protection.partner.outlook.cn -all\n  spf_note: >-\n    Hard-fail (-all) policy delegating to Microsoft 365 operated by 21Vianet (the China\n    instance), consistent with the MX record synyi-com.mail.protection.partner.outlook.cn.\n  dmarc: false\n  dmarc_evidence: no TXT record returned for _dmarc.synyi.com\n  mx:\n  - ' 1 synyi-com.mail.protection.partner.outlook.cn.'\nsummary: >-\n  TLS is correctly deployed and SPF is strict, but three controls are absent: HSTS, DMARC and\n  DNSSEC. Absent CAA is also recorded. The absences are valid measured data, not probe failures.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synyi/refs/heads/main/security/synyi-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Healthcare
- Artificial Intelligence
- Machine-Learning
- Natural Language Processing
- Medical Data
- Clinical Decision Support
- Hospital Information Systems
- Big Data
- China
---
