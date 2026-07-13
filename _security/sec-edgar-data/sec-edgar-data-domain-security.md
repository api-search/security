---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 issue "entrust.net"
  - 0 iodef "mailto:CAIssues@sec.gov"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sec.gov
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.sec.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sec Edgar Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SEC EDGAR Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SEC EDGAR Data
provider_slug: sec-edgar-data
slug: sec-edgar-data-domain-security
source_filename: sec-edgar-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sec.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sec.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 issue \"entrust.net\"\n  - 0 iodef \"mailto:CAIssues@sec.gov\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sec-edgar-data/refs/heads/main/security/sec-edgar-data-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Finance
- Public APIs
---
